---
UID: NS:commctrl.__unnamed_struct_11
title: NMCBEDRAGBEGINW
author: windows-sdk-content
description: Contains information used with the CBEN_DRAGBEGIN notification code.
old-location: controls\NMCBEDRAGBEGIN.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\comboex\structures\nmcbedragbegin.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPNMCBEDRAGBEGINW, *PNMCBEDRAGBEGINW, LPNMCBEDRAGBEGIN, LPNMCBEDRAGBEGIN structure pointer [Windows Controls], NMCBEDRAGBEGIN, NMCBEDRAGBEGIN structure [Windows Controls], NMCBEDRAGBEGINA, NMCBEDRAGBEGINW, _win32_NMCBEDRAGBEGIN, _win32_NMCBEDRAGBEGIN_cpp, commctrl/LPNMCBEDRAGBEGIN, commctrl/NMCBEDRAGBEGIN, commctrl/NMCBEDRAGBEGINA, commctrl/NMCBEDRAGBEGINW, controls.NMCBEDRAGBEGIN, controls._win32_NMCBEDRAGBEGIN"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: NMCBEDRAGBEGINW (Unicode) and NMCBEDRAGBEGINA (ANSI)
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
 - NMCBEDRAGBEGIN
 - NMCBEDRAGBEGINA
 - NMCBEDRAGBEGINW
product: Windows
targetos: Windows
req.typenames: NMCBEDRAGBEGINW, *LPNMCBEDRAGBEGINW, *PNMCBEDRAGBEGINW
req.redist: 
---

# NMCBEDRAGBEGINW structure


## -description


Contains information used with the <a href="https://msdn.microsoft.com/bdab2700-a605-48af-aee3-bbf573408e3f">CBEN_DRAGBEGIN</a> notification code. 


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/0c8b116b-82ad-495a-b19d-8c172e0b2608">NMHDR</a></b>

An <a href="https://msdn.microsoft.com/0c8b116b-82ad-495a-b19d-8c172e0b2608">NMHDR</a> structure that contains information about the notification code. 


### -field iItemid

Type: <b>int</b>

The zero-based index of the item being dragged. This value will always be -1, indicating that the item being dragged is the item displayed in the edit portion of the control. 


### -field szText

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">TCHAR</a></b>

The character buffer that contains the text of the item being dragged. 

