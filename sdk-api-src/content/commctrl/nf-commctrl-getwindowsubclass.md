---
UID: NF:commctrl.GetWindowSubclass
title: GetWindowSubclass function
author: windows-sdk-content
description: Retrieves the reference data for the specified window subclass callback.
old-location: shell\GetWindowSubclass.htm
tech.root: shell
ms.assetid: 3969f18e-3e12-4770-8596-2c2c6519c2a7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetWindowSubclass, GetWindowSubclass function [Windows Shell], commctrl/GetWindowSubclass, inet_GetWindowSubclass, shell.GetWindowSubclass
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: commctrl.h
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
req.lib: Comctl32.lib
req.dll: Comctl32.dll (version 6.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Comctl32.dll
api_name:
 - GetWindowSubclass
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetWindowSubclass function


## -description


Retrieves the reference data for the specified window subclass callback.


## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

The handle of the window being subclassed.


### -param pfnSubclass [in]

Type: <b><a href="https://msdn.microsoft.com/44e4cbe0-8252-4bcc-885e-d8af856e8ad7">SUBCLASSPROC</a></b>

A pointer to a window procedure. This pointer and the subclass ID uniquely identify this subclass callback.


### -param uIdSubclass [in]

Type: <b>UINT_PTR</b>

<b>UINT_PTR</b> subclass ID. This ID and the callback pointer uniquely identify this subclass callback. Note: On 64-bit versions of Windows this is a 64-bit value.


### -param pdwRefData [out]

Type: <b>DWORD_PTR*</b>

A pointer to a <b>DWORD</b> which will return the reference data. Note: On 64-bit versions of Windows, pointers are 64-bit values.


## -returns



Type: <b>BOOL</b>

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TRUE</b></dt>
</dl>
</td>
<td width="60%">
The subclass callback was successfully installed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FALSE</b></dt>
</dl>
</td>
<td width="60%">
The subclass callback was not installed.

</td>
</tr>
</table>
 




## -remarks



To use <b>GetWindowSubclass</b>, specify Comctl32.dll version 6 in the manifest. For more information on manifests, see <a href="https://msdn.microsoft.com/en-us/library/Bb773175(v=VS.85).aspx">Enabling Visual Styles</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb776403(v=VS.85).aspx">DefSubclassProc</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb762094(v=VS.85).aspx">RemoveWindowSubclass</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb762102(v=VS.85).aspx">SetWindowSubclass</a>
 

 

