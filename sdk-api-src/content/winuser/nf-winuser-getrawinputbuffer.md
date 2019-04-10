---
UID: NF:winuser.GetRawInputBuffer
title: GetRawInputBuffer function (winuser.h)
author: windows-sdk-content
description: Performs a buffered read of the raw input data.
old-location: inputdev\getrawinputbuffer.htm
tech.root: inputdev
ms.assetid: VS|winui|~\winui\windowsuserinterface\userinput\rawinput\rawinputreference\rawinputfunctions\getrawinputbuffer.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRawInputBuffer, GetRawInputBuffer function [Keyboard and Mouse Input], _win32_GetRawInputBuffer, _win32_getrawinputbuffer_cpp, inputdev.getrawinputbuffer, winui._win32_getrawinputbuffer, winuser/GetRawInputBuffer
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
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
 - GetRawInputBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetRawInputBuffer function


## -description


Performs a buffered read of the raw input data.


## -parameters




### -param pData [out, optional]

Type: <b>PRAWINPUT</b>

A pointer to a buffer of <a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a> structures that contain the raw input data. If <b>NULL</b>, the minimum required buffer, in bytes, is returned in *<i>pcbSize</i>. 


### -param pcbSize [in, out]

Type: <b>PUINT</b>

The size, in bytes, of a <a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a> structure. 


### -param cbSizeHeader [in]

Type: <b>UINT</b>

The size, in bytes, of the <a href="https://msdn.microsoft.com/en-us/library/ms645571(v=VS.85).aspx">RAWINPUTHEADER</a> structure. 


## -returns



Type: <b>UINT</b>

If 
						<i>pData</i> is NULL and the function is successful, the return value is zero. If 
						<i>pData</i> is not NULL and the function is successful, the return value is the number of <a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a> structures written to 
						<i>pData</i>.

If an error occurs, the return value is (<b>UINT</b>)-1. Call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> for the error code.




## -remarks



Using <b>GetRawInputBuffer</b>, the raw input data is buffered in the array of <a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a> structures. For an unbuffered read, use the <a href="https://msdn.microsoft.com/en-us/library/ms644936(v=VS.85).aspx">GetMessage</a> function to read in the raw input data. 

The <a href="https://msdn.microsoft.com/en-us/library/ms645593(v=VS.85).aspx">NEXTRAWINPUTBLOCK</a> macro allows an application to traverse an array of <a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a> structures.

<div class="alert"><b>Note</b>  To get the correct size of the raw input buffer, do not use *<i>pcbSize</i>, use *<i>pcbSize</i> * 8 instead.   To ensure <b>GetRawInputBuffer</b> behaves properly on WOW64, you must align the <a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a> structure by 8 bytes. The following code shows how to align <b>RAWINPUT</b>  for WOW64.  


```
[StructLayout(LayoutKind.Explicit)]
internal struct RAWINPUT
{
    [FieldOffset(0)]
    public RAWINPUTHEADER header;

    [FieldOffset(16+8)]
    public RAWMOUSE mouse;

    [FieldOffset(16+8)]
    public RAWKEYBOARD keyboard;

    [FieldOffset(16+8)]
    public RAWHID hid;
}

```


</div>
<div> </div>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms644936(v=VS.85).aspx">GetMessage</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645593(v=VS.85).aspx">NEXTRAWINPUTBLOCK</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645562(v=VS.85).aspx">RAWINPUT</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645571(v=VS.85).aspx">RAWINPUTHEADER</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645536(v=VS.85).aspx">Raw Input</a>



<b>Reference</b>
 

 

