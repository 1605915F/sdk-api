---
UID: NF:msctf.ITfMouseSink.OnMouseEvent
title: ITfMouseSink::OnMouseEvent
author: windows-sdk-content
description: ITfMouseSink::OnMouseEvent method
old-location: tsf\itfmousesink_onmouseevent.htm
tech.root: TSF
ms.assetid: 1aa4fdb7-b16d-4e58-934a-8323450f6749
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITfMouseSink interface [Text Services Framework],OnMouseEvent method, ITfMouseSink.OnMouseEvent, ITfMouseSink::OnMouseEvent, OnMouseEvent, OnMouseEvent method [Text Services Framework], OnMouseEvent method [Text Services Framework],ITfMouseSink interface, _tsf_itfmousesink_onmouseevent_ref, msctf/ITfMouseSink::OnMouseEvent, tsf.itfmousesink_onmouseevent
ms.topic: method
req.header: msctf.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
req.dll: Msctf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msctf.dll
api_name:
 - ITfMouseSink.OnMouseEvent
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfMouseSink::OnMouseEvent


## -description




## -parameters




### -param uEdge [in]

Contains the offset, in characters, of the mouse position from the start of the range of text. For more information, see the Remarks section.


### -param uQuadrant [in]

Contains the zero-based quadrant index, relative to the edge, that the mouse position lies in. For more information, see the Remarks section.


### -param dwBtnStatus [in]

Indicates the mouse button state at the time of the event. See the <i>wParam</i> parameter of the <a href="https://msdn.microsoft.com/en-us/library/ms645616(v=VS.85).aspx">WM_MOUSEMOVE</a> message for possible values.


### -param pfEaten [out]

Pointer to a BOOL that, on exit, indicates if the mouse event was handled. If this value receives <b>TRUE</b>, the mouse event was handled. If this value is <b>FALSE</b>, the mouse event was not handled.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
</table>
 




## -remarks



The caller should translate double-click events into multiple mouse button down events. This enables a text service to detect double-click events even if the context window does not support double-clicks.

<i>uEdge</i> contains the offset, in characters, of the mouse position from the start of the text range. The mouse position is always rounded to the closest edge. Each edge is divided into four equal quadrants with two quadrants preceding the edge and two quadrants following the edge. <i>uQuadrant</i> contains the zero-based quadrant index of the mouse position. In the figure below, point "X" is in quadrant 2 of edge 1 and point "Y" is in quadrant 1 of edge 3.

<img alt="Quadrant relationship to edge of a range of text" border="border" src="./images/mousedge.gif"/>



## -see-also




<a href="https://msdn.microsoft.com/d6e5549e-768d-47af-a553-84430641cda4">ITfMouseSink</a>



<a href="https://msdn.microsoft.com/d73b2b9b-8904-4507-9b32-dcb8946fb887">ITfMouseTracker::AdviseMouseSink
      </a>



<a href="https://msdn.microsoft.com/365538cd-0f18-45ce-91c2-ee3255b7fa93">ITfMouseTrackerACP::AdviseMouseSink
      </a>



<a href="https://msdn.microsoft.com/en-us/library/ms645616(v=VS.85).aspx">WM_MOUSEMOVE</a>
 

 

