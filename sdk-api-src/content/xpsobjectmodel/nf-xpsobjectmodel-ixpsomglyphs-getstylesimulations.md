---
UID: NF:xpsobjectmodel.IXpsOMGlyphs.GetStyleSimulations
title: IXpsOMGlyphs::GetStyleSimulations
author: windows-sdk-content
description: Gets the style simulations that will be applied when rendering the glyphs.
old-location: xps\ixpsomglyphs_getstylesimulations.htm
tech.root: printdocs
ms.assetid: 5678f67e-ed26-4846-b2f7-4e7f9690ca43
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetStyleSimulations, GetStyleSimulations method [XPS Documents and Packaging], GetStyleSimulations method [XPS Documents and Packaging],IXpsOMGlyphs interface, IXpsOMGlyphs interface [XPS Documents and Packaging],GetStyleSimulations method, IXpsOMGlyphs.GetStyleSimulations, IXpsOMGlyphs::GetStyleSimulations, xps.ixpsomglyphs_getstylesimulations, xpsobjectmodel/IXpsOMGlyphs::GetStyleSimulations
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
 - IXpsOMGlyphs.GetStyleSimulations
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMGlyphs::GetStyleSimulations


## -description


Gets the style simulations that will  be applied when rendering the glyphs.


## -parameters




### -param styleSimulations [out, retval]

The <a href="https://msdn.microsoft.com/3f77c349-ba78-44e9-866a-9f654ed0e9dd">XPS_STYLE_SIMULATION</a> value that describes the style simulations to be applied.


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
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<i>styleSimulations</i> is <b>NULL</b>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/6d2cda65-c719-46f2-97c9-8aee7b5f84b9">IXpsOMGlyphs</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>



<a href="https://msdn.microsoft.com/3f77c349-ba78-44e9-866a-9f654ed0e9dd">XPS_STYLE_SIMULATION</a>
 

 

