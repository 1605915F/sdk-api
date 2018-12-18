---
UID: NF:winver.GetFileVersionInfoSizeA
title: GetFileVersionInfoSizeA function
author: windows-sdk-content
description: Determines whether the operating system can retrieve version information for a specified file. If version information is available, GetFileVersionInfoSize returns the size, in bytes, of that information.
old-location: menurc\getfileversioninfosize.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\versioninformation\versioninformationreference\versioninformationfunctions\getfileversioninfosize.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetFileVersionInfoSize, GetFileVersionInfoSize function [Menus and Other Resources], GetFileVersionInfoSizeA, GetFileVersionInfoSizeW, _win32_GetFileVersionInfoSize, _win32_getfileversioninfosize_cpp, menurc.getfileversioninfosize, winui._win32_getfileversioninfosize, winver/GetFileVersionInfoSize, winver/GetFileVersionInfoSizeA, winver/GetFileVersionInfoSizeW
ms.topic: function
req.header: winver.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: GetFileVersionInfoSizeW (Unicode) and GetFileVersionInfoSizeA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mincore.lib
req.dll: Api-ms-win-core-version-l1-1-0.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - api-ms-win-core-version-l1-1-0.dll
 - API-MS-Win-Core-Versionansi-L1-1-1.dll
 - API-MS-Win-Core-Version-L1-1-1.dll
 - KernelBase.dll
 - version.dll
api_name:
 - GetFileVersionInfoSize
 - GetFileVersionInfoSizeA
 - GetFileVersionInfoSizeW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetFileVersionInfoSizeA function


## -description


Determines whether the operating system can retrieve version information for a specified file. If version information is available, <b>GetFileVersionInfoSize</b> returns the size, in bytes, of that information. 


## -parameters




### -param lptstrFilename [in]

Type: <b>LPCTSTR</b>

The name of the file of interest. The function uses the search sequence specified by the  <a href="https://msdn.microsoft.com/d936b4dd-058c-48e1-834b-b47ef6d8ef65">LoadLibrary</a> function.
				


### -param lpdwHandle [out, optional]

Type: <b>LPDWORD</b>

A pointer to a variable that the function sets to zero.


## -returns



Type: <b>DWORD</b>

If the function succeeds, the return value is the size, in bytes, of the file's version information.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -remarks



Call the 
				<b>GetFileVersionInfoSize</b> function before calling the <a href="https://msdn.microsoft.com/en-us/library/ms647003(v=VS.85).aspx">GetFileVersionInfo</a> function. The size returned by <b>GetFileVersionInfoSize</b> indicates the buffer size required for the version information returned by <b>GetFileVersionInfo</b>. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647003(v=VS.85).aspx">GetFileVersionInfo</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647001(v=VS.85).aspx">VS_VERSIONINFO</a>



<a href="https://msdn.microsoft.com/en-us/library/ms647464(v=VS.85).aspx">VerQueryValue</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646981(v=VS.85).aspx">Version Information</a>
 

 

