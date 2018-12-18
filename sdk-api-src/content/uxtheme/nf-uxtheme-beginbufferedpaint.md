---
UID: NF:uxtheme.BeginBufferedPaint
title: BeginBufferedPaint function
author: windows-sdk-content
description: Begins a buffered paint operation.
old-location: controls\BeginBufferedPaint.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\userex\functions\beginbufferedpaint.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BeginBufferedPaint, BeginBufferedPaint function [Windows Controls], _shell_BeginBufferedPaint, _shell_BeginBufferedPaint_cpp, controls.BeginBufferedPaint, controls._shell_BeginBufferedPaint, uxtheme/BeginBufferedPaint
ms.topic: function
req.header: uxtheme.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: UxTheme.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - UxTheme.dll
 - ext-ms-win-uxtheme-themes-l1-1-1.dll
 - xamlpalwp.dll
api_name:
 - BeginBufferedPaint
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# BeginBufferedPaint function


## -description


Begins a buffered paint operation.


## -parameters




### -param hdcTarget

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HDC</a></b>

The handle of the target DC on which the buffer will be painted.


### -param prcTarget

Type: <b>const <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that specifies the area of the target DC in which to paint.


### -param dwFormat

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb759835(v=VS.85).aspx">BP_BUFFERFORMAT</a></b>

A member of the <a href="https://msdn.microsoft.com/en-us/library/Bb759835(v=VS.85).aspx">BP_BUFFERFORMAT</a> enumeration that specifies the format of the buffer.


### -param pPaintParams [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb773228(v=VS.85).aspx">BP_PAINTPARAMS</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/Bb773228(v=VS.85).aspx">BP_PAINTPARAMS</a> structure that defines the paint operation parameters. This value can be <b>NULL</b>.


### -param phdc [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HDC</a>*</b>

When this function returns, points to the handle of the new device context.


## -returns



Type: <b>HPAINTBUFFER</b>

A handle to the buffered paint context. If this function fails, the return value is <b>NULL</b>, and <i>phdc</i> is <b>NULL</b>. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.

The returned handle is freed when <a href="https://msdn.microsoft.com/en-us/library/Bb773343(v=VS.85).aspx">EndBufferedPaint</a> is called.

An application should call <a href="https://msdn.microsoft.com/en-us/library/Bb773266(v=VS.85).aspx">BufferedPaintInit</a> on the calling thread before calling <b>BeginBufferedPaint</b>, and <a href="https://msdn.microsoft.com/en-us/library/Bb773284(v=VS.85).aspx">BufferedPaintUnInit</a> before the thread is terminated.  Failure to call <b>BufferedPaintInit</b> may result in degraded performance due to internal data being initialized and destroyed for each buffered paint operation.



