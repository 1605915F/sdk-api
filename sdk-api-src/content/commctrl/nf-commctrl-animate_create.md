---
UID: NF:commctrl.Animate_Create
title: Animate_Create macro
author: windows-sdk-content
description: Creates an animation control. Animate_Create calls the CreateWindow function to create the animation control.
old-location: controls\Animate_Create.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\animation\macros\animate_create.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Animate_Create, Animate_Create macro [Windows Controls], _win32_Animate_Create, _win32_Animate_Create_cpp, commctrl/Animate_Create, controls.Animate_Create, controls._win32_Animate_Create
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
 - Animate_Create
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Animate_Create macro


## -description


Creates an animation control. <b>Animate_Create</b> calls the <a href="https://msdn.microsoft.com/en-us/library/ms632679(v=VS.85).aspx">CreateWindow</a> function to create the animation control. 


## -parameters




### -param hwndP

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the parent window. 


### -param id

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The child window identifier of the animation control. 


### -param dwStyle

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

The window styles. For a list of the animation control style values, see <a href="https://msdn.microsoft.com/en-us/library/Bb761886(v=VS.85).aspx">Animation Control Styles</a>. 


### -param hInstance

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HINSTANCE</a></b>

A handle to the instance of the module that is creating the animation control. 


## -remarks



The <b>Animate_Create</b> macro sets the width and height of the animation control to zero if the <a href="https://msdn.microsoft.com/en-us/library/Bb761886(v=VS.85).aspx">ACS_CENTER</a> style is specified. If the <b>ACS_CENTER</b> style is not specified, <b>Animate_Create</b> sets the width and height based on the dimensions of a frame in the AVI clip. 



