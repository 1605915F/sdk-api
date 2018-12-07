---
UID: NF:winuser.DrawIcon
title: DrawIcon function
author: windows-sdk-content
description: Draws an icon or cursor into the specified device context.
old-location: menurc\drawicon.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\icons\iconreference\iconfunctions\drawicon.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DrawIcon, DrawIcon function [Menus and Other Resources], _win32_DrawIcon, _win32_drawicon_cpp, menurc.drawicon, winui._win32_drawicon, winuser/DrawIcon
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
api_name:
 - DrawIcon
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DrawIcon function


## -description


Draws an icon or cursor into the specified device context.

To specify additional drawing options, use the <a href="https://msdn.microsoft.com/en-us/library/ms648065(v=VS.85).aspx">DrawIconEx</a> function.


## -parameters




### -param hDC [in]

Type: <b>HDC</b>

A handle to the device context into which the icon or cursor will be drawn. 


### -param X [in]

Type: <b>int</b>

The logical x-coordinate of the upper-left corner of the icon. 


### -param Y [in]

Type: <b>int</b>

The logical y-coordinate of the upper-left corner of the icon. 


### -param hIcon [in]

Type: <b>HICON</b>

A handle to the icon to be drawn. 


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -remarks



<b>DrawIcon</b> places the icon's upper-left corner at the location specified by the <i>X</i> and <i>Y</i> parameters. The location is subject to the current mapping mode of the device context. 

<b>DrawIcon</b> draws the icon or cursor using the width and height specified by the system metric values for icons; for more information, see <a href="https://msdn.microsoft.com/d063857b-6036-4e68-80af-9c70d12ae29e">GetSystemMetrics</a>.


#### Examples

For an example, see <a href="https://msdn.microsoft.com/en-us/library/ms648051(v=VS.85).aspx">Displaying an Icon</a>.

<div class="code"></div>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms648059(v=VS.85).aspx">CreateIcon</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648065(v=VS.85).aspx">DrawIconEx</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646973(v=VS.85).aspx">Icons</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648072(v=VS.85).aspx">LoadIcon</a>



<b>Reference</b>
 

 

