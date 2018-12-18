---
UID: NS:ddrawint._DD_D3DBUFCALLBACKS
title: DD_D3DBUFCALLBACKS
author: windows-sdk-content
description: The DD_D3DBUFCALLBACKS structure is used only by drivers that implement driver level allocation of command and vertex buffers.
old-location: display\dd_d3dbufcallbacks.htm
tech.root: display
ms.assetid: 59fa4043-6238-49f7-b9d6-58c1f215865a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PDD_D3DBUFCALLBACKS, DD_D3DBUFCALLBACKS, DD_D3DBUFCALLBACKS structure [Display Devices], PDD_D3DBUFCALLBACKS, PDD_D3DBUFCALLBACKS structure pointer [Display Devices], ddrawint/DD_D3DBUFCALLBACKS, ddrawint/PDD_D3DBUFCALLBACKS, ddstrcts_cfe891c1-2660-460f-ac58-79f243ee902e.xml, display.dd_d3dbufcallbacks"
ms.topic: struct
req.header: ddrawint.h
req.include-header: Winddi.h
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
 - ddrawint.h
api_name:
 - DD_D3DBUFCALLBACKS
product: Windows
targetos: Windows
req.typenames: DD_D3DBUFCALLBACKS, *PDD_D3DBUFCALLBACKS
req.redist: 
---

# DD_D3DBUFCALLBACKS structure


## -description


The DD_D3DBUFCALLBACKS structure is used only by drivers that implement driver level allocation of command and vertex buffers.


## -struct-fields




### -field dwSize

Specifies the size in bytes of this DD_D3DBUFCALLBACKS structure.


### -field dwFlags

Reserved.


### -field CanCreateD3DBuffer

Points to the driver's <a href="https://msdn.microsoft.com/94aace9f-0927-4b33-a9ea-79c27d5edea9">CanCreateD3DBuffer</a> callback.


### -field CreateD3DBuffer

Points to the driver's <a href="https://msdn.microsoft.com/8b012e65-b78b-41a4-ac05-d9be015b6ed8">CreateD3DBuffer</a> callback.


### -field DestroyD3DBuffer

Points to the driver's <a href="https://msdn.microsoft.com/f86c5c86-f0f2-4e2e-9235-a675d950bce1">DestroyD3DBuffer</a> callback.


### -field LockD3DBuffer

Points to the driver's <a href="https://msdn.microsoft.com/8e0714df-1ac8-448c-9f0f-d361640c133a">LockD3DBuffer</a> callback.


### -field UnlockD3DBuffer

Points to the driver's <a href="https://msdn.microsoft.com/ab0476f5-64da-415e-a8aa-ccbfc9f1a082">UnlockD3DBuffer</a> callback.


## -remarks



Drivers that manage their own command and vertex buffers must fill out a DD_D3DBUFCALLBACKS structure and point the <b>lpD3DBufCallbacks</b> member of <a href="https://msdn.microsoft.com/99ecd219-1e85-4904-867d-3efcb378bb11">DD_HALINFO</a> to it. 

The driver must also support the callback functions reported in the DD_D3DBUFCALLBACKS structure. These <i>XxxD3DBuffer</i> callbacks are each analogous to the <i>DdXxxSurface</i> callback of similar name; they have the same prototypes and are called with the same input parameters. These new callbacks are called only when the surface in question has the DDSCAPS_EXECUTEBUFFER flag set in the surface caps. The buffer creation flags are DDSCAPS_WRITEONLY, DDSCAPS2_VERTEXBUFFER and DDSCAPS2_COMMANDBUFFER. 

The driver determines the type of buffer being requested by checking the <b>ddsCaps</b> member of the <a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a> structure that is passed to <a href="https://msdn.microsoft.com/94aace9f-0927-4b33-a9ea-79c27d5edea9">CanCreateD3DBuffer</a> and <a href="https://msdn.microsoft.com/8b012e65-b78b-41a4-ac05-d9be015b6ed8">CreateD3DBuffer</a> for the following flags:

<ul>
<li>
DDSCAPS_VERTEXBUFFER

Indicates that the driver should allocate an explicit vertex buffer.

</li>
<li>
DDSCAPS_COMMANDBUFFER

Indicates that the driver should allocate a command buffer. 

</li>
<li>
The absence of both these flags 

Indicates that the driver should allocate an implicit vertex buffer.

</li>
</ul>
Implicit vertex buffers should not be placed in video memory because they are expected to be read/write. Only explicit vertex buffers with the DDSCAPS_WRITEONLY flag set can be safely placed in video memory.




## -see-also




<a href="https://msdn.microsoft.com/94aace9f-0927-4b33-a9ea-79c27d5edea9">CanCreateD3DBuffer</a>



<a href="https://msdn.microsoft.com/8b012e65-b78b-41a4-ac05-d9be015b6ed8">CreateD3DBuffer</a>



<a href="https://msdn.microsoft.com/99ecd219-1e85-4904-867d-3efcb378bb11">DD_HALINFO</a>



<a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a>



<a href="https://msdn.microsoft.com/f86c5c86-f0f2-4e2e-9235-a675d950bce1">DestroyD3DBuffer</a>



<a href="https://msdn.microsoft.com/8e0714df-1ac8-448c-9f0f-d361640c133a">LockD3DBuffer</a>



<a href="https://msdn.microsoft.com/ab0476f5-64da-415e-a8aa-ccbfc9f1a082">UnlockD3DBuffer</a>
 

 

