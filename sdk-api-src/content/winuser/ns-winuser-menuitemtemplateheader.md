---
UID: NS:winuser.__unnamed_struct_6
title: MENUITEMTEMPLATEHEADER
author: windows-sdk-content
description: Defines the header for a menu template. A complete menu template consists of a header and one or more menu item lists.
old-location: menurc\menuitemtemplateheader.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\menus\menureference\menustructures\menuitemtemplateheader.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMENUITEMTEMPLATEHEADER, MENUITEMTEMPLATEHEADER, MENUITEMTEMPLATEHEADER structure [Menus and Other Resources], PMENUITEMTEMPLATEHEADER, PMENUITEMTEMPLATEHEADER structure pointer [Menus and Other Resources], _win32_MENUITEMTEMPLATEHEADER_str, _win32_menuitemtemplateheader_str_cpp, menurc.menuitemtemplateheader, winui._win32_menuitemtemplateheader_str, winuser/MENUITEMTEMPLATEHEADER, winuser/PMENUITEMTEMPLATEHEADER"
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
 - MENUITEMTEMPLATEHEADER
product: Windows
targetos: Windows
req.typenames: MENUITEMTEMPLATEHEADER, *PMENUITEMTEMPLATEHEADER
req.redist: 
---

# MENUITEMTEMPLATEHEADER structure


## -description


Defines the header for a menu template. A complete menu template consists of a header and one or more menu item lists. 


## -struct-fields




### -field versionNumber

Type: <b>WORD</b>

The version number. This member must be zero. 


### -field offset

Type: <b>WORD</b>

The offset, in bytes, from the end of the header. The menu item list begins at this offset. Usually, this member is zero, and the menu item list follows immediately after the header. 


## -remarks



One or more <a href="https://msdn.microsoft.com/en-us/library/ms647581(v=VS.85).aspx">MENUITEMTEMPLATE</a> structures are combined to form the menu item list. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647991(v=VS.85).aspx">LoadMenuIndirect</a>



<a href="https://msdn.microsoft.com/en-us/library/ms647581(v=VS.85).aspx">MENUITEMTEMPLATE</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646977(v=VS.85).aspx">Menus</a>



<b>Reference</b>
 

 

