---
UID: NS:ddkmapi._DDREGISTERCALLBACK
title: DDREGISTERCALLBACK
author: windows-sdk-content
description: The DDREGISTERCALLBACK structure contains the register callback information. This structure is used by both the DD_DXAPI_REGISTER_CALLBACK and DD_DXAPI_UNREGISTER_CALLBACK function identifiers of the DxApi function.
old-location: display\ddregistercallback.htm
tech.root: display
ms.assetid: 35b82122-0cff-4a19-9723-28ce38896f2a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDDREGISTERCALLBACK, DDREGISTERCALLBACK, DDREGISTERCALLBACK structure [Display Devices], LPDDREGISTERCALLBACK, LPDDREGISTERCALLBACK structure pointer [Display Devices], ddkmapi/DDREGISTERCALLBACK, ddkmapi/LPDDREGISTERCALLBACK, ddstrcts_bf4e1fea-7c5d-4ae9-96bf-39a78d184aa5.xml, display.ddregistercallback"
ms.topic: struct
req.header: ddkmapi.h
req.include-header: Ddkmapi.h
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
 - HeaderDef
api_location:
 - ddkmapi.h
api_name:
 - DDREGISTERCALLBACK
product: Windows
targetos: Windows
req.typenames: DDREGISTERCALLBACK, *LPDDREGISTERCALLBACK
req.redist: 
---

# DDREGISTERCALLBACK structure


## -description


The DDREGISTERCALLBACK structure contains the register callback information. This structure is used by both the <a href="https://msdn.microsoft.com/62132334-8989-48cb-919e-a236d2c53683">DD_DXAPI_REGISTER_CALLBACK</a> and <a href="https://msdn.microsoft.com/f6850d7d-3e46-4dc6-b8fd-ddb3dc7994d1">DD_DXAPI_UNREGISTER_CALLBACK</a> function identifiers of the <b>DxApi</b> function. 


## -struct-fields




### -field hDirectDraw

Specifies the Microsoft DirectDraw handle.


### -field dwEvents

Defines the event that should trigger the callback. The values in <b>dwParam1</b> and <b>dwParam2</b> depend on the event. The following events are defined:

<table>
<tr>
<th>Event</th>
<th>Description</th>
<th>dwParam1,dwParam2</th>
</tr>
<tr>
<td>
DDEVENT_DISPLAY_VSYNC

</td>
<td>
Called every time a display V-sync occurs.

</td>
<td>

<dl>
<dt>unused,</dt>
<dt>unused</dt>
</dl>


</td>
</tr>
<tr>
<td>
DDEVENT_POSTDOSBOX

</td>
<td>
Called after returning from a full-screen MS-DOS box or the security dialog box (appears when CTRL+ALT+DELETE is pressed).

</td>
<td>

<dl>
<dt>unused,</dt>
<dt>unused</dt>
</dl>


</td>
</tr>
<tr>
<td>
DDEVENT_POSTRESCHANGE

</td>
<td>
Called after a mode change occurs.

</td>
<td>

<dl>
<dt>unused,</dt>
<dt>unused</dt>
</dl>


</td>
</tr>
<tr>
<td>
DDEVENT_PREDOSBOX

</td>
<td>
Called before entering a full-screen MS-DOS box or the security dialog box (appears when CTRL+ALT+DELETE is pressed).

</td>
<td>

<dl>
<dt>unused,</dt>
<dt>unused</dt>
</dl>


</td>
</tr>
<tr>
<td>
DDEVENT_PRERESCHANGE

</td>
<td>
Called before a mode change occurs.

</td>
<td>

<dl>
<dt>unused,</dt>
<dt>unused</dt>
</dl>


</td>
</tr>
<tr>
<td>
DDEVENT_VP_LINE

</td>
<td>
Sets an IRQ to occur each time the hardware video port writes the specified line and then calls the callback each time the IRQ is triggered.

</td>
<td>

<dl>
<dt>hVideoPort,</dt>
<dt>line</dt>
</dl>


</td>
</tr>
<tr>
<td>
DDEVENT_VP_VSYNC

</td>
<td>
Called each time a hardware video port V-sync occurs.

</td>
<td>

<dl>
<dt>hVideoPort,</dt>
<dt>unused</dt>
</dl>


</td>
</tr>
</table>
 


### -field pfnCallback

Points to a <a href="https://msdn.microsoft.com/ee581d7b-c3b8-47e5-bae8-348b22ea0f95">pfnCallback</a> callback function that is called when the event that is specified by the <b>dwEvents</b> member occurs.


### -field dwParam1

Defined by the <b>dwEvents</b> member.


### -field dwParam2

Defined by the <b>dwEvents</b> member.


### -field pContext

Contains client data that is passed back to the client if the <b>pfnCallback</b> callback function is called.


## -see-also




<a href="https://msdn.microsoft.com/62132334-8989-48cb-919e-a236d2c53683">DD_DXAPI_REGISTER_CALLBACK</a>



<a href="https://msdn.microsoft.com/f6850d7d-3e46-4dc6-b8fd-ddb3dc7994d1">DD_DXAPI_UNREGISTER_CALLBACK</a>



<a href="https://msdn.microsoft.com/c4b38376-b54f-4fbb-b305-5951a1ea76a1">DxApi</a>
 

 

