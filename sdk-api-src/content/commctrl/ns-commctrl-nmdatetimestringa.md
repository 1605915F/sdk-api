---
UID: NS:commctrl.tagNMDATETIMESTRINGA
title: NMDATETIMESTRINGA
author: windows-sdk-content
description: Contains information specific to an edit operation that has taken place in a date and time picker (DTP) control. This message is used with the DTN_USERSTRING notification code.
old-location: controls\NMDATETIMESTRING.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\datetime\structures\nmdatetimestring.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPNMDATETIMESTRINGA, LPNMDATETIMESTRING, LPNMDATETIMESTRING structure pointer [Windows Controls], NMDATETIMESTRING, NMDATETIMESTRING structure [Windows Controls], NMDATETIMESTRINGA, NMDATETIMESTRINGW, _win32_NMDATETIMESTRING, _win32_NMDATETIMESTRING_cpp, commctrl/LPNMDATETIMESTRING, commctrl/NMDATETIMESTRING, commctrl/NMDATETIMESTRINGA, commctrl/NMDATETIMESTRINGW, controls.NMDATETIMESTRING, controls._win32_NMDATETIMESTRING"
ms.topic: struct
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: NMDATETIMESTRINGW (Unicode) and NMDATETIMESTRINGA (ANSI)
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
 - NMDATETIMESTRING
 - NMDATETIMESTRINGA
 - NMDATETIMESTRINGW
product: Windows
targetos: Windows
req.typenames: NMDATETIMESTRINGA, *LPNMDATETIMESTRINGA
req.redist: 
---

# NMDATETIMESTRINGA structure


## -description


Contains information specific to an edit operation that has taken place in a date and time picker (DTP) control. This message is used with the <a href="https://msdn.microsoft.com/en-us/library/Bb761745(v=VS.85).aspx">DTN_USERSTRING</a> notification code. 


## -struct-fields




### -field nmhdr

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a></b>

An <a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> structure that contains information about this notification code. 


### -field pszUserString

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCTSTR</a></b>

The address of the zero-terminated string that the user entered. 


### -field st

Type: <b><a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a></b>

A <a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a> structure that must be filled in by the owner when handling the <a href="https://msdn.microsoft.com/en-us/library/Bb761745(v=VS.85).aspx">DTN_USERSTRING</a> notification code. 


### -field dwFlags

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

The return field. Set this member to GDT_VALID to indicate that the 
					<b>st</b> member is valid or to GDT_NONE to set the control to "no date" status (<a href="https://msdn.microsoft.com/en-us/library/Bb761728(v=VS.85).aspx">DTS_SHOWNONE</a> style only). 

