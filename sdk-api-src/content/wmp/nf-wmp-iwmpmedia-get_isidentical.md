---
UID: NF:wmp.IWMPMedia.get_isIdentical
title: IWMPMedia::get_isIdentical
author: windows-sdk-content
description: The get_isIdentical method retrieves a value indicating whether the specified object is the same as the current one.
old-location: wmp\iwmpmedia_get_isidentical.htm
tech.root: WMP
ms.assetid: 6ec54350-0359-4759-a6ba-6132ce33feff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPMedia interface [Windows Media Player],get_isIdentical method, IWMPMedia.get_isIdentical, IWMPMedia2 interface [Windows Media Player],get_isIdentical method, IWMPMedia2::get_isIdentical, IWMPMedia3 interface [Windows Media Player],get_isIdentical method, IWMPMedia3::get_isIdentical, IWMPMedia::get_isIdentical, IWMPMediaget_isIdentical, get_isIdentical, get_isIdentical method [Windows Media Player], get_isIdentical method [Windows Media Player],IWMPMedia interface, get_isIdentical method [Windows Media Player],IWMPMedia2 interface, get_isIdentical method [Windows Media Player],IWMPMedia3 interface, wmp.iwmpmedia_get_isidentical, wmp/IWMPMedia2::get_isIdentical, wmp/IWMPMedia3::get_isIdentical, wmp/IWMPMedia::get_isIdentical
ms.topic: method
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 9 Series or later.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Wmp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmp.dll
api_name:
 - IWMPMedia.get_isIdentical
 - IWMPMedia2.get_isIdentical
 - IWMPMedia3.get_isIdentical
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPMedia::get_isIdentical


## -description



The <b>get_isIdentical</b> method retrieves a value indicating whether the specified object is the same as the current one.




## -parameters




### -param pIWMPMedia [in]

Pointer to an <b>IWMPMedia</b> object that this method will compare to the current object.


### -param pvbool [out]

Pointer to a <b>VARIANT_BOOL</b> that indicates whether the objects were identical.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd563397(v=VS.85).aspx">IWMPMedia Interface</a>
 

 

