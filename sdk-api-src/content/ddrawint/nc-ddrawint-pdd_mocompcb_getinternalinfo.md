---
UID: NC:ddrawint.PDD_MOCOMPCB_GETINTERNALINFO
title: PDD_MOCOMPCB_GETINTERNALINFO (ddrawint.h)
author: windows-sdk-content
description: The DdMoCompGetInternalInfo callback function allows the driver to report that it internally allocates display memory to perform motion compensation.
old-location: display\ddmocompgetinternalinfo.htm
tech.root: display
ms.assetid: 297ff4a2-52f4-4b24-9abe-9c7d22a9b3ad
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DdMoCompGetInternalInfo, DdMoCompGetInternalInfo callback function [Display Devices], PDD_MOCOMPCB_GETINTERNALINFO, PDD_MOCOMPCB_GETINTERNALINFO callback, ddfncs_0dc5afc5-0e35-49eb-a376-afbfe5def553.xml, ddrawint/DdMoCompGetInternalInfo, display.ddmocompgetinternalinfo
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
 - DdMoCompGetInternalInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PDD_MOCOMPCB_GETINTERNALINFO callback function


## -description


The <b>DdMoCompGetInternalInfo</b> callback function allows the driver to report that it internally allocates display memory to perform motion compensation. 


## -parameters




### -param Arg1








#### - lpInternalData

Points to a <a href="https://msdn.microsoft.com/5d8f722f-7574-485e-9ff2-568cd0ae23f7">DD_GETINTERNALMOCOMPDATA</a> structure that contains the internal memory requirements.


## -returns



<b>DdMoCompGetInternalInfo</b> returns one of the following callback codes:




## -remarks



DirectDraw drivers that support motion compensation must implement <b>DdMoCompGetInternalInfo</b>.

This function allows the decoder and DirectShow to make better-informed decisions regarding what GUID to choose.




## -see-also




<a href="https://msdn.microsoft.com/5d8f722f-7574-485e-9ff2-568cd0ae23f7">DD_GETINTERNALMOCOMPDATA</a>
 

 

