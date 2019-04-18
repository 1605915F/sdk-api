---
UID: NS:fwptypes.FWPM_DISPLAY_DATA0_
title: FWPM_DISPLAY_DATA0 (fwptypes.h)
author: windows-sdk-content
description: Stores an optional friendly name and an optional description for an object.
old-location: fwp\fwpm_display_data0_struct.htm
tech.root: fwp
ms.assetid: b86ca572-b4f4-4d40-adfd-fb0e9d32fcd5
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FWPM_DISPLAY_DATA0, FWPM_DISPLAY_DATA0 structure [Filtering], FWPM_DISPLAY_DATA0_, fwp.fwpm_display_data0_struct, fwptypes/FWPM_DISPLAY_DATA0
ms.topic: struct
req.header: fwptypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - Fwptypes.h
api_name:
 - FWPM_DISPLAY_DATA0
product: Windows
targetos: Windows
req.typenames: FWPM_DISPLAY_DATA0
req.redist: 
ms.custom: 19H1
---

# FWPM_DISPLAY_DATA0 structure


## -description


The <b>FWPM_DISPLAY_DATA0</b> structure stores an optional friendly name and an optional description for an object. 


## -struct-fields




### -field name

 Optional friendly name.


### -field description

Optional description.


## -remarks



In order to
support MUI, both strings may contain indirect strings. See
<a href="https://msdn.microsoft.com/en-us/library/Bb759919(v=VS.85).aspx">SHLoadIndirectString</a> for details.

<b>FWPM_DISPLAY_DATA0</b> is a specific implementation of FWPM_DISPLAY_DATA. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a>  for more information.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb759919(v=VS.85).aspx">SHLoadIndirectString</a>



<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 

