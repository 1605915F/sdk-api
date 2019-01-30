---
UID: NF:strmif.IMediaFilter.Pause
title: IMediaFilter::Pause
author: windows-sdk-content
description: The Pause method pauses the filter.
old-location: dshow\imediafilter_pause.htm
tech.root: DirectShow
ms.assetid: 0dbd79be-8f44-4bac-b117-03e6316693f8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBaseFilter interface [DirectShow],Pause method, IBaseFilter::Pause, IMediaFilter interface [DirectShow],Pause method, IMediaFilter.Pause, IMediaFilter::Pause, IMediaFilterPause, Pause, Pause method [DirectShow], Pause method [DirectShow],IBaseFilter interface, Pause method [DirectShow],IMediaFilter interface, dshow.imediafilter_pause, strmif/IBaseFilter::Pause, strmif/IMediaFilter::Pause
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IMediaFilter.Pause
 - IBaseFilter.Pause
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMediaFilter::Pause


## -description



The <b>Pause</b> method pauses the filter. 




## -parameters






## -returns



Returns an <b>HRESULT</b> value. Possible values include those shown in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
Transition is not complete.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success. Transition is complete.

</td>
</tr>
</table>
 




## -remarks



When a filter is paused, it can receive, process, and deliver samples. However, a renderer filter will only accept one sample while paused. Therefore, when the filter graph is paused, samples move through the graph until the first sample reaches the renderer. At that point, streaming is paused until the <a href="https://msdn.microsoft.com/ec422312-bbc2-4b66-b2cd-1a9eebd1eee1">IMediaFilter::Run</a> method is called. Video renderers display the first sample as a still frame.
      

Live capture filters do not deliver any samples while paused, only while running.
      

The state transition might be asynchronous. If the method returns before the transition completes, the return value is <b>S_FALSE</b>. A renderer filter does not complete the transition to paused until either (1) it receives one sample, or (2) it receives an end-of-stream notification. While the state transition is pending, <a href="https://msdn.microsoft.com/b20ca3e9-bec2-4c6d-ba80-f4dae2f5a831">IMediaFilter::GetState</a> returns <b>VFW_S_STATE_INTERMEDIATE</b>.
      




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/d8c09dc7-dae8-4b51-8da8-69e64928a091">IBaseFilter</a>



<a href="https://msdn.microsoft.com/5c0060e8-a9e5-4141-a38d-9a1bc55cc91b">IMediaFilter Interface</a>
 

 

