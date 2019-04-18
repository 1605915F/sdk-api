---
UID: NS:ddrawint._DD_COLORCONTROLCALLBACKS
title: DD_COLORCONTROLCALLBACKS (ddrawint.h)
author: windows-sdk-content
description: The DD_COLORCONTROLCALLBACKS structure contains an entry pointer to the Microsoft DirectDraw color control callback that a device driver supports.
old-location: display\dd_colorcontrolcallbacks.htm
tech.root: display
ms.assetid: fcf0e136-a7cc-4bb3-8af4-2478d4a2c055
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDD_COLORCONTROLCALLBACKS, DD_COLORCONTROLCALLBACKS, DD_COLORCONTROLCALLBACKS structure [Display Devices], PDD_COLORCONTROLCALLBACKS, PDD_COLORCONTROLCALLBACKS structure pointer [Display Devices], ddrawint/DD_COLORCONTROLCALLBACKS, ddrawint/PDD_COLORCONTROLCALLBACKS, ddstrcts_2e14797b-2bd8-4107-8085-60f8b5838bda.xml, display.dd_colorcontrolcallbacks"
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
 - DD_COLORCONTROLCALLBACKS
product: Windows
targetos: Windows
req.typenames: DD_COLORCONTROLCALLBACKS
req.redist: 
ms.custom: 19H1
---

# DD_COLORCONTROLCALLBACKS structure


## -description


The DD_COLORCONTROLCALLBACKS structure contains an entry pointer to the Microsoft DirectDraw color control callback that a device driver supports.


## -struct-fields




### -field dwSize

Specifies the size in bytes of this DD_COLORCONTROLCALLBACKS structure.


### -field dwFlags

Indicates whether the device supports the color control callback identified by <b>ColorControl</b>. The driver should set this member to be DDHAL_COLOR_COLORCONTROL when it implements the color control callback.


### -field ColorControl

Points to the driver-supplied <a href="https://msdn.microsoft.com/626fdd37-bebb-47b7-9899-7cf0dc2bd1ba">DdControlColor</a> callback.


## -remarks



Entries that the display driver does not use should be set to <b>NULL</b>. The driver should initialize this structure when its <a href="https://msdn.microsoft.com/89a22163-a678-4c72-932a-ae4d17922e0b">DdGetDriverInfo</a> function is called with the GUID_ColorControlCallbacks GUID.




## -see-also




<a href="https://msdn.microsoft.com/d68b2772-dca6-417a-8e03-d3b2843fb69d">DD_CALLBACKS</a>



<a href="https://msdn.microsoft.com/85dcb71b-ad1f-4b83-8ead-db502d9f294e">DD_KERNELCALLBACKS</a>



<a href="https://msdn.microsoft.com/9bf47408-cc7f-455d-bbb2-6f1f318eee5f">DD_MISCELLANEOUSCALLBACKS</a>



<a href="https://msdn.microsoft.com/db707fd8-2190-4c4f-89fd-ab46d97f66a2">DD_MOTIONCOMPCALLBACKS</a>



<a href="https://msdn.microsoft.com/9d226b1c-6959-4cc8-9e60-b57a324d9a8a">DD_NTCALLBACKS</a>



<a href="https://msdn.microsoft.com/742b03b0-f729-489c-a87f-b8eb404b6290">DD_PALETTECALLBACKS</a>



<a href="https://msdn.microsoft.com/a363446e-a9f7-4b32-acc2-c369d3dfe8f3">DD_SURFACECALLBACKS</a>



<a href="https://msdn.microsoft.com/5e03d240-f483-4ecf-8890-b9f0368e2b2f">DD_VIDEOPORTCALLBACKS</a>



<a href="https://msdn.microsoft.com/626fdd37-bebb-47b7-9899-7cf0dc2bd1ba">DdControlColor</a>



<a href="https://msdn.microsoft.com/89a22163-a678-4c72-932a-ae4d17922e0b">DdGetDriverInfo</a>
 

 

