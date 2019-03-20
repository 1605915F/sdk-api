---
UID: NS:ddrawint._DD_ADDATTACHEDSURFACEDATA
title: DD_ADDATTACHEDSURFACEDATA (ddrawint.h)
author: windows-sdk-content
description: The DD_ADDATTACHEDSURFACEDATA structure contains information necessary to attach a surface to another surface.
old-location: display\dd_addattachedsurfacedata.htm
tech.root: display
ms.assetid: d00120d9-5825-4998-a1ef-ccc5654b91b9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PDD_ADDATTACHEDSURFACEDATA, DD_ADDATTACHEDSURFACEDATA, DD_ADDATTACHEDSURFACEDATA structure [Display Devices], ddrawint/DD_ADDATTACHEDSURFACEDATA, ddstrcts_2697c197-c588-4f30-8f96-db7d835f3929.xml, display.dd_addattachedsurfacedata"
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
 - DD_ADDATTACHEDSURFACEDATA
product: Windows
targetos: Windows
req.typenames: "*PDD_ADDATTACHEDSURFACEDATA, DD_ADDATTACHEDSURFACEDATA"
req.redist: 
---

# DD_ADDATTACHEDSURFACEDATA structure


## -description


The DD_ADDATTACHEDSURFACEDATA structure contains information necessary to attach a surface to another surface.


## -struct-fields




### -field lpDD

Points to a <a href="https://msdn.microsoft.com/a59f064b-48cf-4491-82cd-84f59467af87">DD_DIRECTDRAW_GLOBAL</a> structure that describes the driver's device.


### -field lpDDSurface

Points to a <a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a> structure that represents the surface to which another surface is being attached.


### -field lpSurfAttached

Points to a DD_SURFACE_LOCAL structure that represents the surface to be attached.


### -field ddRVal

Specifies the location in which the driver writes the return value of the <a href="https://msdn.microsoft.com/53f146e6-f521-4c95-b98b-0e8acb994c9d">DdAddAttachedSurface</a> callback. A return code of DD_OK indicates success. For more information, see <a href="https://msdn.microsoft.com/da4cc7d7-6826-48aa-96c6-004e31fc3e3e">Return Values for DirectDraw</a>.


### -field AddAttachedSurface

Unused on Microsoft Windows 2000 and later.


## -see-also




<a href="https://msdn.microsoft.com/53f146e6-f521-4c95-b98b-0e8acb994c9d">DdAddAttachedSurface</a>
 

 

