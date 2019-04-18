---
UID: NF:vfw.GetSaveFileNamePreviewA
title: GetSaveFileNamePreviewA function (vfw.h)
author: windows-sdk-content
description: The GetSaveFileNamePreview function selects a file by using the Save As dialog box. The dialog box also allows the user to preview the currently specified file. This function augments the capability found in the GetSaveFileName function.
old-location: multimedia\getsavefilenamepreview.htm
tech.root: Multimedia
ms.assetid: f6dd3127-b3fb-40bc-892c-34bacb47d9a6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSaveFileNamePreview, GetSaveFileNamePreview function [Windows Multimedia], GetSaveFileNamePreviewA, GetSaveFileNamePreviewW, _win32_GetSaveFileNamePreview, multimedia.getsavefilenamepreview, vfw/GetSaveFileNamePreview, vfw/GetSaveFileNamePreviewA, vfw/GetSaveFileNamePreviewW
ms.topic: function
req.header: vfw.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: GetSaveFileNamePreviewW (Unicode) and GetSaveFileNamePreviewA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Vfw32.lib
req.dll: Msvfw32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Msvfw32.dll
api_name:
 - GetSaveFileNamePreview
 - GetSaveFileNamePreviewA
 - GetSaveFileNamePreviewW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetSaveFileNamePreviewA function


## -description



The <b>GetSaveFileNamePreview</b> function selects a file by using the Save As dialog box. The dialog box also allows the user to preview the currently specified file. This function augments the capability found in the <a href="http://go.microsoft.com/fwlink/p/?linkid=16940">GetSaveFileName</a> function.




## -parameters




### -param lpofn

Pointer to an <b>OPENFILENAME</b> structure used to initialize the dialog box. On return, the structure contains information about the user's file selection.


## -returns



Returns a handle to the selected file.



