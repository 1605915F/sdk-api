---
UID: NF:winuser.InsertMenuItemW
title: InsertMenuItemW function (winuser.h)
author: windows-sdk-content
description: Inserts a new menu item at the specified position in a menu.
old-location: menurc\insertmenuitem.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\menus\menureference\menufunctions\insertmenuitem.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: InsertMenuItem, InsertMenuItem function [Menus and Other Resources], InsertMenuItemA, InsertMenuItemW, _win32_InsertMenuItem, _win32_insertmenuitem_cpp, menurc.insertmenuitem, winui._win32_insertmenuitem, winuser/InsertMenuItem, winuser/InsertMenuItemA, winuser/InsertMenuItemW
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: InsertMenuItemW (Unicode) and InsertMenuItemA (ANSI)
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
 - Ext-MS-Win-NTUser-Menu-l1-1-1.dll
 - ext-ms-win-ntuser-menu-l1-1-2.dll
 - Ext-MS-Win-NTUser-Menu-L1-1-3.dll
api_name:
 - InsertMenuItem
 - InsertMenuItemA
 - InsertMenuItemW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# InsertMenuItemW function


## -description


Inserts a new menu item at the specified position in a menu.


## -parameters




### -param hmenu [in]

Type: <b>HMENU</b>

A handle to the menu in which the new menu item is inserted. 


### -param item [in]

Type: <b>UINT</b>

The identifier or position of the menu item before which to insert the new item. The meaning of this parameter depends on the value of <i>fByPosition</i>. 


### -param fByPosition [in]

Type: <b>BOOL</b>

Controls the meaning of <i>uItem</i>. If this parameter is <b>FALSE</b>, <i>uItem</i> is a menu item identifier. Otherwise, it is a menu item position. See <a href="https://msdn.microsoft.com/en-us/library/ms647553(v=VS.85).aspx">Accessing Menu Items Programmatically</a> for more information.


### -param lpmi [in]

Type: <b>LPCMENUITEMINFO</b>

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms647578(v=VS.85).aspx">MENUITEMINFO</a> structure that contains information about the new menu item. 


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, use the <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function.




## -remarks



The application must call the <a href="https://msdn.microsoft.com/en-us/library/ms647633(v=VS.85).aspx">DrawMenuBar</a> function whenever a menu changes, whether the menu is in a displayed window.

In order for keyboard accelerators to work with bitmap or owner-drawn menu items, the owner of the menu must process the <a href="https://msdn.microsoft.com/en-us/library/ms646349(v=VS.85).aspx">WM_MENUCHAR</a> message. See <a href="https://msdn.microsoft.com/en-us/library/ms647558(v=VS.85).aspx">Owner-Drawn Menus and the WM_MENUCHAR Message</a> for more information.


#### Examples

For an example, see <a href="https://msdn.microsoft.com/en-us/library/ms647558(v=VS.85).aspx">Example of Menu-Item Bitmaps</a>.

<div class="code"></div>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647633(v=VS.85).aspx">DrawMenuBar</a>



<a href="https://msdn.microsoft.com/en-us/library/ms647578(v=VS.85).aspx">MENUITEMINFO</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646977(v=VS.85).aspx">Menus</a>



<b>Reference</b>
 

 

