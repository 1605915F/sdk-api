---
UID: NN:control.IMediaEvent
title: IMediaEvent (control.h)
author: windows-sdk-content
description: The IMediaEvent interface contains methods for retrieving event notifications and for overriding the Filter Graph Manager's default handling of events.
old-location: dshow\imediaevent.htm
tech.root: DirectShow
ms.assetid: 651561d1-4e7e-48de-9cba-769ddb553e63
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IMediaEvent, IMediaEvent interface [DirectShow], IMediaEvent interface [DirectShow],described, IMediaEventInterface, control/IMediaEvent, dshow.imediaevent
ms.topic: interface
req.header: control.h
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
 - IMediaEvent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMediaEvent interface


## -description



The <code>IMediaEvent</code> interface contains methods for retrieving event notifications and for overriding the Filter Graph Manager's default handling of events. The <a href="https://msdn.microsoft.com/en-us/library/Dd406897(v=VS.85).aspx">IMediaEventEx</a> interface inherits this interface and extends it.

The Filter Graph Manager implements this interface. Applications can use it to respond to events that occur in the filter graph, such as the end of a stream or a rendering error. Filters post events to the filter graph using the <a href="https://msdn.microsoft.com/en-us/library/Dd406901(v=VS.85).aspx">IMediaEventSink</a> interface.

For more information about event notification, see <a href="https://msdn.microsoft.com/301116a5-24e3-4c6d-8c80-bec77c7d62d7">Event Notification in DirectShow</a>. For a list of system-defined event notifications, see <a href="https://msdn.microsoft.com/339ffcd9-7724-4c92-b241-afbed81d9380">Event Notification Codes</a>.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMediaEvent</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IMediaEvent</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMediaEvent</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd406903(v=VS.85).aspx">CancelDefaultHandling</a>
</td>
<td align="left" width="63%">
Cancels the Filter Graph Manager's default handling for a specified event.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd406905(v=VS.85).aspx">FreeEventParams</a>
</td>
<td align="left" width="63%">
Frees resources associated with the parameters of an event.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd406907(v=VS.85).aspx">GetEvent</a>
</td>
<td align="left" width="63%">
Retrieves the next event notification from the event queue.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd406908(v=VS.85).aspx">GetEventHandle</a>
</td>
<td align="left" width="63%">
Retrieves a handle to a manual-reset event that remains signaled while the queue contains event notifications.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd406912(v=VS.85).aspx">RestoreDefaultHandling</a>
</td>
<td align="left" width="63%">
Restores the Filter Graph Manager's default handling for a specified event.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd406914(v=VS.85).aspx">WaitForCompletion</a>
</td>
<td align="left" width="63%">
Waits for the filter graph to render all available data.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

