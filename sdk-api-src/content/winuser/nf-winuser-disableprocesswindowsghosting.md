---
UID: NF:winuser.DisableProcessWindowsGhosting
title: DisableProcessWindowsGhosting function
author: windows-sdk-content
description: Disables the window ghosting feature for the calling GUI process. Window ghosting is a Windows Manager feature that lets the user minimize, move, or close the main window of an application that is not responding.
old-location: winprog\disableprocesswindowsghosting.htm
tech.root: devnotes
ms.assetid: VS|winui|~\winui\windowsuserinterface\lowlevelclientsupport\misc\rtldisableprocesswindowsghosting.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DisableProcessWindowsGhosting, DisableProcessWindowsGhosting function [Windows API], winprog.disableprocesswindowsghosting, winui.disableprocesswindowsghosting, winuser/DisableProcessWindowsGhosting
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winuser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
 - DisableProcessWindowsGhosting
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DisableProcessWindowsGhosting function


## -description


Disables the window ghosting feature for the calling GUI process. Window ghosting is a Windows Manager feature that lets the user minimize, move, or close the main window of an application that is not responding.


## -parameters






## -returns



This function does not return a value.




## -remarks



After calling <b>DisableProcessWindowsGhosting</b>, the ghosting feature is disabled for the duration of the process.


		



