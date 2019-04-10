---
UID: NS:commctrl._HD_TEXTFILTERW
title: HD_TEXTFILTERW (commctrl.h)
author: windows-sdk-content
description: Contains information about header control text filters.
old-location: controls\HDTEXTFILTER.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\header\structures\hdtextfilter.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPHD_TEXTFILTERW, HDTEXTFILTER, HDTEXTFILTER structure [Windows Controls], HD_TEXTFILTERA, HD_TEXTFILTERW, LPHD_TEXTFILTER, LPHD_TEXTFILTER structure pointer [Windows Controls], _HD_TEXTFILTERA, _HD_TEXTFILTERW, _win32_HDTEXTFILTER_Structure, _win32_HDTEXTFILTER_Structure_cpp, commctrl/HDTEXTFILTER, commctrl/LPHD_TEXTFILTER, controls.HDTEXTFILTER, controls._win32_HDTEXTFILTER_Structure"
ms.topic: struct
req.header: commctrl.h
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
 - Commctrl.h
api_name:
 - HDTEXTFILTER
 - HD_TEXTFILTERA
 - HD_TEXTFILTERW
product: Windows
targetos: Windows
req.typenames: HD_TEXTFILTERW, *LPHD_TEXTFILTERW
req.redist: 
---

# HD_TEXTFILTERW structure


## -description


Contains information about header control text filters. 


## -struct-fields




### -field pszText

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPTSTR</a></b>

A pointer to the buffer containing the filter. 


### -field cchTextMax

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">INT</a></b>

A value specifying the maximum size, in characters, for an edit control buffer. 

