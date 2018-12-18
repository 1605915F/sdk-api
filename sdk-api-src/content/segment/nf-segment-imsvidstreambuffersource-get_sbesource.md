---
UID: NF:segment.IMSVidStreamBufferSource.get_SBESource
title: IMSVidStreamBufferSource::get_SBESource
author: windows-sdk-content
description: The get_SBESource method retrieves a pointer to the Stream Buffer Source filter.
old-location: mstv\imsvidstreambuffersource_get_sbesource.htm
tech.root: mstv
ms.assetid: 6ba9cf64-bf26-4a17-ae7a-3e92fc67138d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidStreamBufferSource interface [Microsoft TV Technologies],get_SBESource method, IMSVidStreamBufferSource.get_SBESource, IMSVidStreamBufferSource::get_SBESource, IMSVidStreamBufferSourceget_SBESource, get_SBESource, get_SBESource method [Microsoft TV Technologies], get_SBESource method [Microsoft TV Technologies],IMSVidStreamBufferSource interface, mstv.imsvidstreambuffersource_get_sbesource, segment/IMSVidStreamBufferSource::get_SBESource
ms.topic: method
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Segment.idl
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
 - segment.h
api_name:
 - IMSVidStreamBufferSource.get_SBESource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidStreamBufferSource::get_SBESource


## -description


The <b>get_SBESource</b> method retrieves a pointer to the <a href="https://msdn.microsoft.com/435081e9-8a3f-42ab-9091-30c7c3dd59c6">Stream Buffer Source</a> filter.


## -parameters




### -param sbeFilter [out]

Receives a pointer to the filter's <b>IUnknown</b> interface.
          


## -returns



The method returns an <b>HRESULT</b>. Possible values include the following.

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
 




## -remarks



The caller must release the <b>IUnknown</b> interface.
      




## -see-also




<a href="https://msdn.microsoft.com/12160959-820b-4534-9392-a13ad229317d">IMSVidStreamBufferSource Interface</a>
 

 

