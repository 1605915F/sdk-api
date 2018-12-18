---
UID: NN:wmsdkidl.IWMIndexer
title: IWMIndexer
author: windows-sdk-content
description: The IWMIndexer interface is used to create an index for ASF files to enable seeking.
old-location: wmformat\iwmindexer.htm
tech.root: wmformat
ms.assetid: 00627b0c-4484-417a-8680-0fd97aac41fe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMIndexer, IWMIndexer interface [windows Media Format], IWMIndexer interface [windows Media Format],described, IWMIndexerInterface, wmformat.iwmindexer, wmsdkidl/IWMIndexer
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
 - IWMIndexer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMIndexer interface


## -description



The <b>IWMIndexer</b> interface is used to create an index for ASF files to enable seeking. An index is created only for a file that contains video, although the indexer can safely be used on files that do not contain any video.

An index is an object in the ASF file that equates video samples with presentation times. This is important because the timing of video frames is not necessarily easily computed from the <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">frame rate</a>.

In addition to the standard temporal index, the indexer object can create indexes based on video frame number and SMPTE time code. For more information about creating these indexes, see <a href="https://msdn.microsoft.com/en-us/library/Dd798533(v=VS.85).aspx">IWMIndexer2::Configure</a>.

This interface can be obtained by using the <a href="https://msdn.microsoft.com/en-us/library/Dd757756(v=VS.85).aspx">WMCreateIndexer</a> function.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMIndexer</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMIndexer</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMIndexer</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd757207(v=VS.85).aspx">Cancel</a>
</td>
<td align="left" width="63%">
Cancels indexing.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd757208(v=VS.85).aspx">StartIndexing</a>
</td>
<td align="left" width="63%">
Initiates indexing.

</td>
</tr>
</table> 

The following interface can be obtained by using the QueryInterface method of this interface.

<table>
<tr>
<th>Interface</th>
<th>IID</th>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Dd798532(v=VS.85).aspx">IWMIndexer2</a>
</td>
<td>IID_IWMIndexer2</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/652e04a5-ed6e-4e92-acf4-55ed82f77ef1">Indexer Object</a>



<a href="https://msdn.microsoft.com/c61a0739-09f2-497f-a2cd-d3f2472738e3">Interfaces</a>
 

 

