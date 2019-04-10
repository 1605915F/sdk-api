---
UID: NF:olectl.OleCreatePictureIndirect
title: OleCreatePictureIndirect function (olectl.h)
author: windows-sdk-content
description: Creates a new picture object initialized according to a PICTDESC structure.
old-location: com\olecreatepictureindirect.htm
tech.root: com
ms.assetid: fb021348-07d4-4974-a71e-abb1b8d760c4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: OleCreatePictureIndirect, OleCreatePictureIndirect function [COM], _ole_OleCreatePictureIndirect, com.olecreatepictureindirect, olectl/OleCreatePictureIndirect
ms.topic: function
req.header: olectl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: OleAut32.lib
req.dll: OleAut32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - OleAut32.dll
api_name:
 - OleCreatePictureIndirect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OleCreatePictureIndirect function


## -description


Creates a new picture object initialized according to a <a href="https://msdn.microsoft.com/eb1f1de7-dcfe-4c1c-8737-f5ab4d7977d6">PICTDESC</a> structure.


## -parameters




### -param lpPictDesc [in]

Pointer to a caller-allocated structure containing the initial state of the picture. The specified structure can be <b>NULL</b> to create an uninitialized object, in the event the picture needs to initialize via <a href="https://msdn.microsoft.com/351e1187-9959-4542-8778-925457c3b8e3">IPersistStream::Load</a>.


### -param riid [in]

Reference to the identifier of the interface describing the type of interface pointer to return in <i>lplpvObj</i>.


### -param fOwn [in]

If <b>TRUE</b>, the picture object is to destroy its picture when the object is destroyed. If <b>FALSE</b>, the caller is responsible for destroying the picture.


### -param lplpvObj [out]

Address of pointer variable that receives the interface pointer requested in riid. Upon successful return, this parameter contains the requested interface pointer on the newly created object. If the call is successful, the caller is responsible for calling <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">Release</a> through this interface pointer when the new object is no longer needed. If the call fails, the value is set to <b>NULL</b>.


## -returns



This function returns S_OK on success. Other possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOINTERFACE</b></dt>
</dl>
</td>
<td width="60%">
The object does not support the interface specified in riid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The address in <i>pPictDesc</i> or <i>lplpvObj</i> is not valid. For example, it may be <b>NULL</b>.


</td>
</tr>
</table>
 




## -remarks



 The <i>fOwn</i> parameter indicates whether the picture is to own the GDI picture handle for the picture it contains, so that the picture object will destroy its picture when the object itself is destroyed. The function returns an interface pointer to the new picture object specified by the caller in the <i>riid</i> parameter. A <a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">QueryInterface</a> is built into this call. The caller is responsible for calling <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">Release</a> through the interface pointer returned.




## -see-also




<a href="https://msdn.microsoft.com/de1847cd-ecc0-4941-9dbc-a60b8ef0b1c1">OleLoadPicture</a>



<a href="https://msdn.microsoft.com/eb1f1de7-dcfe-4c1c-8737-f5ab4d7977d6">PICTDESC</a>
 

 

