---
UID: NF:xpsobjectmodel.IXpsOMGeometryFigure.GetSegmentDataCount
title: IXpsOMGeometryFigure::GetSegmentDataCount (xpsobjectmodel.h)
author: windows-sdk-content
description: Gets the number of segment data points in the figure.
old-location: xps\ixpsomgeometryfigure_getsegmentdatacount.htm
tech.root: printdocs
ms.assetid: 42b68a76-e7fe-49d2-9190-4a4d5e763052
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSegmentDataCount, GetSegmentDataCount method [XPS Documents and Packaging], GetSegmentDataCount method [XPS Documents and Packaging],IXpsOMGeometryFigure interface, IXpsOMGeometryFigure interface [XPS Documents and Packaging],GetSegmentDataCount method, IXpsOMGeometryFigure.GetSegmentDataCount, IXpsOMGeometryFigure::GetSegmentDataCount, xps.ixpsomgeometryfigure_getsegmentdatacount, xpsobjectmodel/IXpsOMGeometryFigure::GetSegmentDataCount
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
 - IXpsOMGeometryFigure.GetSegmentDataCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMGeometryFigure::GetSegmentDataCount


## -description


Gets the number of segment data points in the figure.


## -parameters




### -param segmentDataCount [out, retval]

The number of segment data points. <i>segmentDataCount</i> must not be <b>NULL</b> when the method is called.


## -returns



If the method succeeds, it returns S_OK; otherwise, it returns an <b>HRESULT</b> error code.

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
<i>segmentDataCount</i> is <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



To get the segment data points, call <a href="https://msdn.microsoft.com/e2e6be6f-3a9d-4d39-875f-cd23bc82e74b">GetSegmentData</a>.

For an example of how to use this method in a program, see the code example in <a href="https://msdn.microsoft.com/e2e6be6f-3a9d-4d39-875f-cd23bc82e74b">GetSegmentData</a>.




## -see-also




<a href="https://msdn.microsoft.com/17b302c0-31e3-460b-9771-3f293c94447a">GetSegmentCount</a>



<a href="https://msdn.microsoft.com/e2e6be6f-3a9d-4d39-875f-cd23bc82e74b">GetSegmentData</a>



<a href="https://msdn.microsoft.com/a440c227-33c9-42f9-8f4a-4cbe6281f9ad">GetSegmentTypes</a>



<a href="https://msdn.microsoft.com/e76a14ce-cfc3-4a50-855e-f5779b9fc261">IXpsOMGeometryFigure</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>
 

 

