---
UID: NS:dpa_dsa._DPASTREAMINFO
title: DPASTREAMINFO
author: windows-sdk-content
description: Contains a stream item used by the PFNDPASTREAM callback function.
old-location: controls\DPASTREAMINFO.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\common\structures\dpastreaminfo.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DPASTREAMINFO, DPASTREAMINFO structure [Windows Controls], _win32_DPASTREAMINFO, _win32_DPASTREAMINFO_cpp, controls.DPASTREAMINFO, controls._win32_DPASTREAMINFO, dpa_dsa/DPASTREAMINFO
ms.topic: struct
req.header: dpa_dsa.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - dpa_dsa.h
api_name:
 - DPASTREAMINFO
product: Windows
targetos: Windows
req.typenames: DPASTREAMINFO
req.redist: 
---

# DPASTREAMINFO structure


## -description


Contains a stream item used by the <a href="https://msdn.microsoft.com/en-us/library/Bb775725(v=VS.85).aspx">PFNDPASTREAM</a> callback function. 


## -struct-fields




### -field iPos

Type: <b>int</b>

An index of the item in the DPA. 


### -field pvItem

Type: <b>void*</b>

A void pointer to the item data. 

