---
UID: NF:commctrl.MonthCal_SizeRectToMin
title: MonthCal_SizeRectToMin macro (commctrl.h)
author: windows-sdk-content
description: Calculates how many calendars will fit in the given rectangle, and then returns the minimum size that a rectangle needs to be to fit that number of calendars. You can use this macro or send the MCM_SIZERECTTOMIN message explicitly.
old-location: controls\MonthCal_SizeRectToMin.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\monthcal\macros\monthcal_sizerecttomin.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MonthCal_SizeRectToMin, MonthCal_SizeRectToMin macro [Windows Controls], _shell_MonthCal_SizeRectToMin, _shell_MonthCal_SizeRectToMin_cpp, commctrl/MonthCal_SizeRectToMin, controls.MonthCal_SizeRectToMin, controls._shell_MonthCal_SizeRectToMin
ms.topic: macro
req.header: commctrl.h
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
 - Commctrl.h
api_name:
 - MonthCal_SizeRectToMin
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MonthCal_SizeRectToMin macro


## -description


Calculates how many calendars will fit in the given rectangle, and then returns the minimum size that a rectangle needs to be to fit that number of calendars. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761020(v=VS.85).aspx">MCM_SIZERECTTOMIN</a> message explicitly.


## -parameters




### -param hmc

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to a month calendar control.


### -param prc [in, out]

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a></b>

On entry, contains a pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that describes a region that is greater than or equal to the size necessary to fit the desired number of calendars. When this function returns, contains the minimum <b>RECT</b> structure that fits this number of calendars.

