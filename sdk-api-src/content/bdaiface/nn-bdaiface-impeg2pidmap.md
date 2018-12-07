---
UID: NN:bdaiface.IMPEG2PIDMap
title: IMPEG2PIDMap
author: windows-sdk-content
description: This interface is implemented on each output pin of the MPEG-2 Demultiplexer filter (Demux) and is used in transport stream mode only.
old-location: dshow\impeg2pidmap.htm
tech.root: DirectShow
ms.assetid: 45c09a02-7da8-460a-9a64-f012c2181b94
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMPEG2PIDMap, IMPEG2PIDMap interface [DirectShow], IMPEG2PIDMap interface [DirectShow],described, IMPEG2PIDMapInterface, bdaiface/IMPEG2PIDMap, dshow.impeg2pidmap
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: bdaiface.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - IMPEG2PIDMap
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMPEG2PIDMap interface


## -description



This interface is implemented on each output pin of the <a href="https://msdn.microsoft.com/en-us/library/Dd390715(v=VS.85).aspx">MPEG-2 Demultiplexer</a> filter (Demux) and is used in transport stream mode only. It is called by applications or other filters to associate the pin with one or more Packet IDs (PID). Once a PID has been mapped, the Demux will deliver all packets with that ID to the output pin. This interface is not exposed when the filter is playing back a file (pull-mode).

For program streams, use the <a href="https://msdn.microsoft.com/en-us/library/Dd376629(v=VS.85).aspx">IMPEG2StreamIdMap</a> interface.

<b>OCUR Devices: </b>This interface supports OpenCable Unidirectional Cable Receiver (OCUR) devices. See <a href="https://msdn.microsoft.com/en-us/library/Dd695266(v=VS.85).aspx">OCUR Devices</a>.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMPEG2PIDMap</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IMPEG2PIDMap</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>IMPEG2PIDMap</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd407133(v=VS.85).aspx">EnumPIDMap</a>
</td>
<td align="left" width="63%">
Returns a collection of all the currently mapped PIDs on this pin.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd407134(v=VS.85).aspx">MapPID</a>
</td>
<td align="left" width="63%">
Maps the packets of a specified PID to the pin.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd407135(v=VS.85).aspx">UnmapPID</a>
</td>
<td align="left" width="63%">
Unmaps the PID mapping created in a previous call to <a href="https://msdn.microsoft.com/en-us/library/Dd407134(v=VS.85).aspx">MapPID</a>.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/5efd174f-2eb1-44e6-97e3-b73c7c52fef1">Interfaces</a>
 

 

