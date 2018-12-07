---
UID: NF:winuser.SetMenuDefaultItem
title: SetMenuDefaultItem function
author: windows-sdk-content
description: Sets the default menu item for the specified menu.
old-location: menurc\setmenudefaultitem.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\menus\menureference\menufunctions\setmenudefaultitem.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetMenuDefaultItem, SetMenuDefaultItem function [Menus and Other Resources], _win32_SetMenuDefaultItem, _win32_setmenudefaultitem_cpp, menurc.setmenudefaultitem, winui._win32_setmenudefaultitem, winuser/SetMenuDefaultItem
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
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
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
 - ext-ms-win-ntuser-menu-l1-1-2.dll
 - Ext-MS-Win-NTUser-Menu-L1-1-3.dll
api_name:
 - SetMenuDefaultItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetMenuDefaultItem function


## -description


Sets the default menu item for the specified menu.


## -parameters




### -param hMenu [in]

Type: <b>HMENU</b>

A handle to the menu to set the default item for. 


### -param uItem [in]

Type: <b>UINT</b>

The identifier or position of the new default menu item or -1 for no default item. The meaning of this parameter depends on the value of 
					<i>fByPos</i>. 


### -param fByPos [in]

Type: <b>UINT</b>

The meaning of <i>uItem</i>. If this parameter is <b>FALSE</b>, <i>uItem</i> is a menu item identifier. Otherwise, it is a menu item position. See <a href="https://msdn.microsoft.com/en-us/library/ms647553(v=VS.85).aspx">About Menus</a> for more information.


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, use the <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647976(v=VS.85).aspx">GetMenuDefaultItem</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646977(v=VS.85).aspx">Menus</a>



<b>Reference</b>
 

 

