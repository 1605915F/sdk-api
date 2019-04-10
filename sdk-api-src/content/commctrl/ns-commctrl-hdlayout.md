---
UID: NS:commctrl._HD_LAYOUT
title: HDLAYOUT (commctrl.h)
author: windows-sdk-content
description: Contains information used to set the size and position of a header control. HDLAYOUT is used with the HDM_LAYOUT message. This structure supersedes the HD_LAYOUT structure.
old-location: controls\HDLAYOUT.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\header\structures\hdlayout.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPHDLAYOUT, HDLAYOUT, HDLAYOUT structure [Windows Controls], LPHDLAYOUT, LPHDLAYOUT structure pointer [Windows Controls], _win32_HDLAYOUT, _win32_HDLAYOUT_cpp, commctrl/HDLAYOUT, commctrl/LPHDLAYOUT, controls.HDLAYOUT, controls._win32_HDLAYOUT"
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
 - HDLAYOUT
product: Windows
targetos: Windows
req.typenames: HDLAYOUT, *LPHDLAYOUT
req.redist: 
---

# HDLAYOUT structure


## -description


Contains information used to set the size and position of a header control. <b>HDLAYOUT</b> is used with the <a href="https://msdn.microsoft.com/en-us/library/Bb775353(v=VS.85).aspx">HDM_LAYOUT</a> message. This structure supersedes the 
			<b>HD_LAYOUT</b> structure. 


## -struct-fields




### -field prc

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>*</b>

Structure that contains the coordinates of a rectangle that the header control will occupy. 


### -field pwpos

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms632612(v=VS.85).aspx">WINDOWPOS</a>*</b>

Structure that receives information about the appropriate size and position of the header control. 

