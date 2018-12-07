---
UID: NN:wmsdkidl.IWMWriterPreprocess
title: IWMWriterPreprocess
author: windows-sdk-content
description: The IWMWriterPreprocess interface handles multi-pass encoding.
old-location: wmformat\iwmwriterpreprocess.htm
tech.root: wmformat
ms.assetid: 06803639-3f21-4003-a460-16a0b5cc6d6f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMWriterPreprocess, IWMWriterPreprocess interface [windows Media Format], IWMWriterPreprocess interface [windows Media Format],described, IWMWriterPreprocessInterface, wmformat.iwmwriterpreprocess, wmsdkidl/IWMWriterPreprocess
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: wmsdkidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmsdkidl.h
api_name:
 - IWMWriterPreprocess
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMWriterPreprocess interface


## -description



The <b>IWMWriterPreprocess</b> interface handles multi-pass encoding. By making more than one pass, the writer can obtain better quality with better compression.

An <b>IWMWriterPreprocess</b> interface exists for every instance of the writer object. You can obtain a pointer to <b>IWMWriterPreprocess</b> with a call to the <b>QueryInterface</b> method of any other interface in the writer object.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMWriterPreprocess</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMWriterPreprocess</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMWriterPreprocess</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/593aaa1f-b0eb-43a0-bf73-e90225c07cdf">BeginPreprocessingPass</a>
</td>
<td align="left" width="63%">
Begins preprocessing a stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/04ec12fb-946b-46cc-aa3f-515a86b9a217">EndPreprocessingPass</a>
</td>
<td align="left" width="63%">
Ends preprocessing a stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6acdc536-8b38-4fd4-9705-f4399dfc3faa">GetMaxPreprocessingPasses</a>
</td>
<td align="left" width="63%">
Retrieves the maximum number of preprocessing passes supported for a specified stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/95223ace-0c74-48d8-b49a-98b27c7b735f">PreprocessSample</a>
</td>
<td align="left" width="63%">
Retrieves a sample for preprocessing.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/81ff36e1-cce5-4c99-bf3a-ee2f1050c026">SetNumPreprocessingPasses</a>
</td>
<td align="left" width="63%">
Sets the number of preprocessing passes to perform.

</td>
</tr>
</table> 

For information about which interfaces can be obtained by using the QueryInterface method of this interface, see <a href="https://msdn.microsoft.com/8058b7fe-7d02-4572-ad43-6867d4ceb7e9">Writer Object</a>.



## -see-also




<a href="https://msdn.microsoft.com/c61a0739-09f2-497f-a2cd-d3f2472738e3">Interfaces</a>



<a href="https://msdn.microsoft.com/55fc768b-15f0-4236-ad0d-3792ccaa9b4f">Using Two-Pass Encoding</a>



<a href="https://msdn.microsoft.com/8058b7fe-7d02-4572-ad43-6867d4ceb7e9">Writer Object</a>
 

 

