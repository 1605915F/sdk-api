---
UID: NS:winuser.tagMDINEXTMENU
title: tagMDINEXTMENU
author: windows-sdk-content
description: Contains information about the menu to be activated.
old-location: menurc\mdinextmenu.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\menus\menureference\menustructures\mdinextmenu.htm
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: "*LPMDINEXTMENU, *PMDINEXTMENU, MDINEXTMENU, MDINEXTMENU structure [Menus and Other Resources], PMDINEXTMENU, PMDINEXTMENU structure pointer [Menus and Other Resources], _win32_MDINEXTMENU_str, _win32_mdinextmenu_str_cpp, menurc.mdinextmenu, tagMDINEXTMENU, winui._win32_mdinextmenu_str, winuser/MDINEXTMENU, winuser/PMDINEXTMENU"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winuser.h
req.include-header: Windows.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Winuser.h
api_name:
 - MDINEXTMENU
product: Windows
targetos: Windows
req.typenames: MDINEXTMENU, *PMDINEXTMENU, *LPMDINEXTMENU
req.redist: 
---

# tagMDINEXTMENU structure


## -description


Contains information about the menu to be activated. 


## -struct-fields




### -field hmenuIn

Type: <b>HMENU</b>

A handle to the current menu. 


### -field hmenuNext

Type: <b>HMENU</b>

A handle to the menu to be activated. 


### -field hwndNext

Type: <b>HWND</b>

A handle to the window to receive the menu notification messages. 


## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms646977(v=VS.85).aspx">Menus</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647612(v=VS.85).aspx">WM_NEXTMENU</a>
 

 

