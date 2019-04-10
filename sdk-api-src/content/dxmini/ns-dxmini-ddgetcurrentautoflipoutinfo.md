---
UID: NS:dxmini._DDGETCURRENTAUTOFLIPOUTINFO
title: DDGETCURRENTAUTOFLIPOUTINFO (dxmini.h)
author: windows-sdk-content
description: The DDGETCURRENTAUTOFLIPOUTINFO structure provides the surface information.
old-location: display\ddgetcurrentautoflipoutinfo.htm
tech.root: display
ms.assetid: 2dea32ab-9f4a-4184-9979-1103f1b26730
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDDGETCURRENTAUTOFLIPOUTINFO, DDGETCURRENTAUTOFLIPOUTINFO, DDGETCURRENTAUTOFLIPOUTINFO structure [Display Devices], PDDGETCURRENTAUTOFLIPOUTINFO, PDDGETCURRENTAUTOFLIPOUTINFO structure pointer [Display Devices], Video_Structs_2e52113e-1796-45bf-bd0b-d0e373679f15.xml, display.ddgetcurrentautoflipoutinfo, dxmini/DDGETCURRENTAUTOFLIPOUTINFO, dxmini/PDDGETCURRENTAUTOFLIPOUTINFO"
ms.topic: struct
req.header: dxmini.h
req.include-header: Dxmini.h
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
 - dxmini.h
api_name:
 - DDGETCURRENTAUTOFLIPOUTINFO
product: Windows
targetos: Windows
req.typenames: DDGETCURRENTAUTOFLIPOUTINFO, *PDDGETCURRENTAUTOFLIPOUTINFO
req.redist: 
---

# DDGETCURRENTAUTOFLIPOUTINFO structure


## -description


The DDGETCURRENTAUTOFLIPOUTINFO structure provides the surface information. 


## -struct-fields




### -field dwSurfaceIndex

Specifies the current zero-based index in the autoflip chain of the current surface. 


### -field dwVBISurfaceIndex

Specifies the current zero-based index in the autoflip chain of the current <a href="https://msdn.microsoft.com/a1de1905-09f3-4689-ace9-06690a1f930a">vertical blanking interval (VBI)</a> surface. 


## -see-also




<a href="https://msdn.microsoft.com/25010ffb-893f-401f-8883-f5a08e7014bf">DxGetCurrentAutoflip</a>
 

 

