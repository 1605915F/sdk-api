---
UID: NF:olectl.OleLoadPictureEx
title: OleLoadPictureEx function
author: windows-sdk-content
description: Creates a new picture object and initializes it from the contents of a stream. This is equivalent to calling OleCreatePictureIndirect with NULL as the first parameter, followed by a call to IPersistStream::Load.
old-location: com\oleloadpictureex.htm
tech.root: com
ms.assetid: c903096f-f15f-4a36-8efc-20cf7102e77d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OleLoadPictureEx, OleLoadPictureEx function [COM], _ole_OleLoadPictureEx, com.oleloadpictureex, olectl/OleLoadPictureEx
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - OleLoadPictureEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OleLoadPictureEx function


## -description


Creates a new picture object and initializes it from the contents of a stream. This is equivalent to calling <a href="https://msdn.microsoft.com/fb021348-07d4-4974-a71e-abb1b8d760c4">OleCreatePictureIndirect</a> with <b>NULL</b> as the first parameter, followed by a call to <a href="https://msdn.microsoft.com/351e1187-9959-4542-8778-925457c3b8e3">IPersistStream::Load</a>.


## -parameters




### -param lpstream [in]

Pointer to the stream that contains the picture's data.


### -param lSize [in]

The number of bytes that should be read from the stream, or zero if the entire stream should be read.


### -param fRunmode [in]

The opposite of the initial value of the <a href="https://msdn.microsoft.com/90befcb7-138f-4c63-a6ec-ec06c89b3317">KeepOriginalFormat</a> property. If <b>TRUE</b>, <a href="https://msdn.microsoft.com/04d952cf-a3c0-4220-9d24-8188ce52f862">KeepOriginalFormat</a> is set to <b>FALSE</b> and vice versa.


### -param riid [in]

Reference to the identifier of the interface describing the type of interface pointer to return in <i>ppvObj</i>.


### -param xSizeDesired [in]

Desired width of icon or cursor. Valid values are 16, 32, and 48. Pass LP_DEFAULT to both size parameters to use system default size.


### -param ySizeDesired [in]

Desired height of icon or cursor. Valid values are 16, 32, and 48. Pass LP_DEFAULT to both size parameters to use system default size.


### -param dwFlags [in]

Desired color depth for icon or cursor. Values are LP_MONOCHROME (monochrome), LP_VGACOLOR (16 colors), LP_COLOR (256 colors), or LP_DEFAULT (selects best depth for current display).


### -param lplpvObj [out]

Address of pointer variable that receives the interface pointer requested in riid. Upon successful return, *<i>ppvObj</i> contains the requested interface pointer on the storage of the object identified by the moniker. If *<i>ppvObj</i> is non-<b>NULL</b>, this function calls <a href="https://msdn.microsoft.com/b4316efd-73d4-4995-b898-8025a316ba63">IUnknown::AddRef</a> on the interface; it is the caller's responsibility to call <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">IUnknown::Release</a>. If an error occurs, *<i>ppvObj</i> is set to <b>NULL</b>.


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
The address in <i>pPictDesc</i> or <i>ppvObj</i> is not valid. For example, it may be <b>NULL</b>.


</td>
</tr>
</table>
 




## -remarks



The stream must be in BMP (bitmap), WMF (metafile), or ICO (icon) format. A picture object created using <b>OleLoadPictureEx</b> always has ownership of its internal resources (<i>fOwn</i>==<b>TRUE</b> is implied).

In addition to allowing specification of icon or cursor size, <b>OleLoadPictureEx</b> supports loading of color cursors.




## -see-also




<a href="https://msdn.microsoft.com/fb021348-07d4-4974-a71e-abb1b8d760c4">OleCreatePictureIndirect</a>



<a href="https://msdn.microsoft.com/eb1f1de7-dcfe-4c1c-8737-f5ab4d7977d6">PICTDESC</a>
 

 

