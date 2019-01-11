---
UID: NF:dciman.DCICreatePrimary
title: DCICreatePrimary function
author: windows-sdk-content
description: Creates a primary surface and obtains surface information.
old-location: winprog\_dciman_dcicreateprimary.htm
tech.root: DevNotes
ms.assetid: VS|winui|~\winui\windowsuserinterface\lowlevelclientsupport\graphics\dcicreateprimary.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DCICreatePrimary, DCICreatePrimary function [Windows API], _dciman_dcicreateprimary, dciman/DCICreatePrimary, winprog._dciman_dcicreateprimary, winui._dciman_dcicreateprimary
ms.topic: function
req.header: dciman.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dciman32.lib
req.dll: Dciman32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dciman32.dll
api_name:
 - DCICreatePrimary
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DCICreatePrimary function


## -description


<p class="CCE_Message">[This function is subject to change with each operating system revision. Instead, use the Microsoft DirectDraw and Microsoft Direct3DAPIs; these APIs insulate applications from such operating system changes, and hide many other difficulties involved in interacting directly with display drivers.]

Creates a primary surface and obtains surface information.



## -parameters




### -param hdc [in]

The device context handle of the device for the primary surface to be created.


### -param lplpSurface [out]

A pointer to a <b>DCISURFACEINFO</b> structure.


## -returns



If the function succeeds, DCI_OK is returned.  Otherwise, it returns one of the DCI errors.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms648408(v=VS.85).aspx">Graphics Low Level Client Support</a>
 

 

