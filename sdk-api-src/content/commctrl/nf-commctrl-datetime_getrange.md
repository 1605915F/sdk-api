---
UID: NF:commctrl.DateTime_GetRange
title: DateTime_GetRange macro
author: windows-sdk-content
description: Gets the current minimum and maximum allowable system times for a date and time picker (DTP) control. You can use this macro, or send the DTM_GETRANGE message explicitly.
old-location: controls\DateTime_GetRange.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\datetime\macros\datetime_getrange.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DateTime_GetRange, DateTime_GetRange macro [Windows Controls], _win32_DateTime_GetRange, _win32_DateTime_GetRange_cpp, commctrl/DateTime_GetRange, controls.DateTime_GetRange, controls._win32_DateTime_GetRange
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: macro
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
 - DateTime_GetRange
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DateTime_GetRange macro


## -description


Gets the current minimum and maximum allowable system times for a date and time picker (DTP) control. You can use this macro, or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761767(v=VS.85).aspx">DTM_GETRANGE</a> message explicitly. 


## -parameters




### -param hdp

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">HWND</a></b>

A handle to a DTP control.


### -param rgst

Type: <b>LPSYSTEMTIME</b>

A pointer to a two-element array of <a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a> structures. 


## -remarks



The date and time picker displays only dates/times that fall within the specified range, preventing the user from selecting a date and time that falls outside the range. If the <a href="https://msdn.microsoft.com/en-us/library/Bb761813(v=VS.85).aspx">DateTime_SetSystemtime</a> message specifies a date and time that falls outside the range, it will fail.



