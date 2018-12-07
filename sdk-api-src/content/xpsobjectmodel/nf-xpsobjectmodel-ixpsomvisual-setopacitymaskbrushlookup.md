---
UID: NF:xpsobjectmodel.IXpsOMVisual.SetOpacityMaskBrushLookup
title: IXpsOMVisual::SetOpacityMaskBrushLookup
author: windows-sdk-content
description: Sets the lookup key name of a shared opacity mask brush in a resource dictionary.
old-location: xps\ixpsomvisual_setopacitymaskbrushlookup.htm
tech.root: printdocs
ms.assetid: 93c76649-dc48-4ccf-b1c5-2fb223c93513
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXpsOMVisual interface [XPS Documents and Packaging],SetOpacityMaskBrushLookup method, IXpsOMVisual.SetOpacityMaskBrushLookup, IXpsOMVisual::SetOpacityMaskBrushLookup, SetOpacityMaskBrushLookup, SetOpacityMaskBrushLookup method [XPS Documents and Packaging], SetOpacityMaskBrushLookup method [XPS Documents and Packaging],IXpsOMVisual interface, xps.ixpsomvisual_setopacitymaskbrushlookup, xpsobjectmodel/IXpsOMVisual::SetOpacityMaskBrushLookup
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: xpsobjectmodel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XpsObjectModel.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - xpsobjectmodel.h
api_name:
 - IXpsOMVisual.SetOpacityMaskBrushLookup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMVisual::SetOpacityMaskBrushLookup


## -description


Sets the lookup key name of a shared opacity mask brush in a resource dictionary.


## -parameters




### -param key [in]

The lookup key name of the opacity mask brush in the dictionary.  A <b>NULL</b> pointer clears the previously assigned key name.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the table that follows. For information about  XPS document API return values that are not listed in this table, see <a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>.

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
<tr>
<td width="40%">
<dl>
<dt><b>XPS_E_INVALID_RESOURCE_KEY</b></dt>
</dl>
</td>
<td width="60%">
According to the <a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>, the value of <i>lookup</i> is not a valid lookup key string.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>XPS_E_INVALID_LOOKUP_TYPE</b></dt>
</dl>
</td>
<td width="60%">
The lookup key name in <i>key</i> references an object that is not a geometry.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>XPS_E_LOOKUP_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
No object could be found with a key name that matched the value passed in <i>key</i>.

</td>
</tr>
</table>
 




## -remarks



After you call <b>SetOpacityMaskBrushLookup</b>, the local opacity mask brush is released and <a href="https://msdn.microsoft.com/654dc003-25a6-4186-9c3b-7fe6f82b5481">GetOpacityMaskBrushLocal</a> returns a <b>NULL</b> pointer in the <i>opacityMaskBrush</i> parameter. The table that follows explains the relationship between the local and lookup values of this property.


<table>
<tr>
<th>Most recent method called</th>
<th>Object that is returned in <i>opacityMaskBrush</i> by <a href="https://msdn.microsoft.com/df5b770e-cc66-45ee-b865-2959255920bf">GetOpacityMaskBrush</a>
</th>
<th>Object that is returned in <i>opacityMaskBrush</i> by <a href="https://msdn.microsoft.com/654dc003-25a6-4186-9c3b-7fe6f82b5481">GetOpacityMaskBrushLocal</a>
</th>
<th>String that is  returned in <i>key</i> by <a href="https://msdn.microsoft.com/84d4aae9-e3e3-4c82-8877-b8206d3678f0">GetOpacityMaskBrushLookup</a>
</th>
</tr>
<tr>
<td>

<a href="https://msdn.microsoft.com/d1b84156-b7ad-4dac-97d9-60aaedcee210">SetOpacityMaskBrushLocal</a>


</td>
<td>
The local opacity mask brush that is set by <a href="https://msdn.microsoft.com/d1b84156-b7ad-4dac-97d9-60aaedcee210">SetOpacityMaskBrushLocal</a>.

</td>
<td>
The local opacity mask brush that is set by <a href="https://msdn.microsoft.com/d1b84156-b7ad-4dac-97d9-60aaedcee210">SetOpacityMaskBrushLocal</a>.

</td>
<td>
<b>NULL</b> pointer.

</td>
</tr>
<tr>
<td>
<b>SetOpacityMaskBrushLookup</b> (this method)

</td>
<td>
The shared opacity mask brush that gets retrieved—with a lookup key that matches the key that is set by <b>SetOpacityMaskBrushLookup</b>—from the resource directory.

</td>
<td>
<b>NULL</b> pointer.

</td>
<td>
The lookup key that is set by <b>SetOpacityMaskBrushLookup</b>.

</td>
</tr>
<tr>
<td>
Neither <a href="https://msdn.microsoft.com/d1b84156-b7ad-4dac-97d9-60aaedcee210">SetOpacityMaskBrushLocal</a> nor <b>SetOpacityMaskBrushLookup</b> has been called yet.

</td>
<td>
<b>NULL</b> pointer.

</td>
<td>
<b>NULL</b> pointer.

</td>
<td>
<b>NULL</b> pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/f2ec412c-aece-4b20-a721-e6c17615e56b">IXpsOMVisual</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>
 

 

