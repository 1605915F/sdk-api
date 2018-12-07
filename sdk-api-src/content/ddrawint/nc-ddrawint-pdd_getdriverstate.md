---
UID: NC:ddrawint.PDD_GETDRIVERSTATE
title: PDD_GETDRIVERSTATE
author: windows-sdk-content
description: The D3dGetDriverState function is used by both the Microsoft DirectDraw and Microsoft Direct3D runtimes to obtain information from the driver about its current state.
old-location: display\d3dgetdriverstate.htm
tech.root: display
ms.assetid: 6e1b0bce-1ac5-46e7-ae25-b0d3ce8580a0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3dGetDriverState, D3dGetDriverState callback function [Display Devices], PDD_GETDRIVERSTATE, PDD_GETDRIVERSTATE callback, d3dfncs_e2c93c0f-5d2e-47b2-b8df-b527db9b121e.xml, ddrawint/D3dGetDriverState, display.d3dgetdriverstate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: ddrawint.h
req.include-header: Winddi.h
req.target-type: Desktop
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
 - UserDefined
api_location:
 - ddrawint.h
api_name:
 - D3dGetDriverState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PDD_GETDRIVERSTATE callback function


## -description


The <i>D3dGetDriverState</i> function is used by both the Microsoft DirectDraw and Microsoft Direct3D runtimes to obtain information from the driver about its current state.


## -parameters




### -param Arg1








#### - pgdsd

Points to a <a href="https://msdn.microsoft.com/a8b02b56-1733-467b-bd11-0185e6778d34">DD_GETDRIVERSTATEDATA</a> structure that describes the state of the driver.


## -returns



<i>D3dGetDriverState</i> returns one of the following callback codes: 




## -remarks



All Direct3D drivers must support <i>D3dGetDriverState</i>.




## -see-also




<a href="https://msdn.microsoft.com/a8b02b56-1733-467b-bd11-0185e6778d34">DD_GETDRIVERSTATEDATA</a>
 

 

