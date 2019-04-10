---
UID: NN:msctf.ITfCompartmentEventSink
title: ITfCompartmentEventSink (msctf.h)
author: windows-sdk-content
description: The ITfCompartmentEventSink interface is implemented by a client (application or text service) and used by the TSF manager to notify the client when compartment data changes.
old-location: tsf\itfcompartmenteventsink.htm
tech.root: TSF
ms.assetid: 1bd464e7-9e34-4725-83f9-42e09ddf4778
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITfCompartmentEventSink, ITfCompartmentEventSink interface [Text Services Framework], ITfCompartmentEventSink interface [Text Services Framework],described, _tsf_itfcompartmenteventsink_ref, msctf/ITfCompartmentEventSink, tsf.itfcompartmenteventsink
ms.topic: interface
req.header: msctf.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Msctf.idl
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
 - Msctf.h
api_name:
 - ITfCompartmentEventSink
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfCompartmentEventSink interface


## -description


The <b>ITfCompartmentEventSink</b> interface is implemented by a client (application or text service) and used by the TSF manager to notify the client when compartment data changes. This notification sink is installed by obtaining an <a href="https://msdn.microsoft.com/2ff77f09-1b4c-4115-9bb4-4040097d1f90">ITfSource</a> interface from the <a href="https://msdn.microsoft.com/c9ca3eb5-1fb1-4e45-9ec4-a0296f1bc8c3">ITfCompartment</a> object and calling <a href="https://msdn.microsoft.com/90928e6e-e11e-42ad-9b3e-d974642aca36">ITfSource::AdviseSink</a> with IID_ITfCompartmentEventSink and a pointer to the <b>ITfCompartmentEventSink</b> object.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITfCompartmentEventSink</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>ITfCompartmentEventSink</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ITfCompartmentEventSink</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1756754c-6353-4296-bdb5-1cbef1d29ec5">OnChange</a>
</td>
<td align="left" width="63%">
Called when compartment data changes.

</td>
</tr>
</table> 

