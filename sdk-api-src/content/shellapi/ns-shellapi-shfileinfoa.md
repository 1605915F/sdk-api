---
UID: NS:shellapi._SHFILEINFOA
title: SHFILEINFOA (shellapi.h)
author: windows-sdk-content
description: Contains information about a file object.
old-location: shell\SHFILEINFO.htm
tech.root: shell
ms.assetid: 9dbf873a-b447-4579-961e-20f2a64c87fe
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SHFILEINFO, SHFILEINFO structure [Windows Shell], SHFILEINFOA, _win32_SHFILEINFO, shell.SHFILEINFO, shellapi/SHFILEINFO
ms.topic: struct
req.header: shellapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
 - Shellapi.h
api_name:
 - SHFILEINFO
product: Windows
targetos: Windows
req.typenames: SHFILEINFOA
req.redist: 
---

# SHFILEINFOA structure


## -description


Contains information about a file object.


## -struct-fields




### -field hIcon

Type: <b>HICON</b>

A handle to the icon that represents the file. You are responsible for destroying this handle with <a href="https://msdn.microsoft.com/en-us/library/ms648063(v=VS.85).aspx">DestroyIcon</a> when you no longer need it.


### -field iIcon

Type: <b>int</b>

The index of the icon image within the system image list.


### -field dwAttributes

Type: <b>DWORD</b>

An array of values that indicates the attributes of the file object. For information about these values, see the <a href="https://msdn.microsoft.com/3864b386-7653-4661-880c-e96c08ff0dbb">IShellFolder::GetAttributesOf</a> method.


### -field szDisplayName

Type: <b>TCHAR[MAX_PATH]</b>

A string that contains the name of the file as it appears in the Windows Shell, or the path and file name of the file that contains the icon representing the file.


### -field szTypeName

Type: <b>TCHAR[80]</b>

A string that describes the type of file.


## -remarks



This structure is used with the <a href="https://msdn.microsoft.com/d662bedf-4be0-4528-8121-e7923a42bc67">SHGetFileInfo</a> function.



