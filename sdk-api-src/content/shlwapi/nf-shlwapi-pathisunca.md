---
UID: NF:shlwapi.PathIsUNCA
title: PathIsUNCA function
author: windows-sdk-content
description: Determines if a path string is a valid Universal Naming Convention (UNC) path, as opposed to a path based on a drive letter.
old-location: shell\PathIsUNC.htm
tech.root: shell
ms.assetid: 53da5ba7-a2a4-45b2-90e0-ae006415933e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PathIsUNC, PathIsUNC function [Windows Shell], PathIsUNCA, PathIsUNCW, _win32_PathIsUNC, shell.PathIsUNC, shlwapi/PathIsUNC, shlwapi/PathIsUNCA, shlwapi/PathIsUNCW
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: shlwapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: PathIsUNCW (Unicode) and PathIsUNCA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Shlwapi.lib
req.dll: Shlwapi.dll (version 4.71 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Shlwapi.dll
 - API-MS-Win-Core-shlwapi-legacy-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-DownLevel-shlwapi-l1-1-0.dll
 - API-MS-Win-DownLevel-shlwapi-l1-1-1.dll
api_name:
 - PathIsUNC
 - PathIsUNCA
 - PathIsUNCW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PathIsUNCA function


## -description


Determines if a path string is a valid Universal Naming Convention (UNC) path, as opposed to a path based on a drive letter.


## -parameters




### -param pszPath [in]

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string of maximum length MAX_PATH that contains the path to validate.


## -returns



Type: <b>BOOL</b>

Returns <b>TRUE</b> if the string is a valid UNC path; otherwise, <b>FALSE</b>.




## -see-also




<a href="https://msdn.microsoft.com/3b2a4158-63ec-49eb-a031-7493d02f2caa">PathIsUNCEx</a>
 

 

