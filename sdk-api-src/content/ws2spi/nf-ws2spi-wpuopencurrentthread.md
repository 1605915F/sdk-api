---
UID: NF:ws2spi.WPUOpenCurrentThread
title: WPUOpenCurrentThread function
author: windows-sdk-content
description: The WPUOpenCurrentThread function opens a handle to the current thread that can be used with overlapped functions in a layered service provider.
old-location: winsock\wpuopencurrentthread_2.htm
tech.root: winsock
ms.assetid: 92d21f29-240f-407e-89a7-bbbb8f9bf0eb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WPUOpenCurrentThread, WPUOpenCurrentThread function [Winsock], _win32_wpuopencurrentthread_2, winsock.wpuopencurrentthread_2, ws2spi/WPUOpenCurrentThread
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: ws2spi.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Ws2spi.h
api_name:
 - WPUOpenCurrentThread
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WPUOpenCurrentThread function


## -description


The 
<b>WPUOpenCurrentThread</b> function opens a handle to the current thread that can be used with overlapped functions in a layered service provider. This is intended to be used by layered service providers that wish to initiate overlapped I/O from nonapplication threads.


## -parameters




### -param lpThreadId [out]

Pointer to a 
<a href="https://msdn.microsoft.com/eeea1139-1d14-4f53-bd64-833539b53bed">WSATHREADID</a> structure that can then be passed to an overlapped function.


### -param lpErrno [out]

Pointer to the error code.


## -returns



If no error occurs, 
<b>WPUOpenCurrentThread</b> returns the zero. Otherwise, it returns SOCKET_ERROR, and a specific error code is available in <i>lpErrno</i>.



<table>
<tr>
<th>Error code</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSANOTINITIALISED</a></b></dt>
</dl>
</td>
<td width="60%">
A successful 
<a href="https://msdn.microsoft.com/9ebfe81c-bed6-4bde-b1dd-5eaefbaac9cf">WSPStartup</a> call must occur before using this function.

</td>
</tr>
</table>
 


<div> </div>





## -remarks



The 
<b>WPUOpenCurrentThread</b> function provides a pointer to a 
<a href="https://msdn.microsoft.com/eeea1139-1d14-4f53-bd64-833539b53bed">WSATHREADID</a> structure that can then be passed to an overlapped function such as 
<a href="https://msdn.microsoft.com/4d741663-34f5-41b9-ba8f-77d45382d50b">WSPSend</a> or 
<a href="https://msdn.microsoft.com/5304a5d6-bc99-4a6f-8eeb-668bbd93fc84">WSPRecv</a>. Layered service providers using a private thread in one of the upper layers will use 
<b>WPUOpenCurrentThread</b> to pass a 
<b>WSATHREADID</b> pointer to the lower layer that is administering overlapped functions.

Overlapped functions such as 
<a href="https://msdn.microsoft.com/4d741663-34f5-41b9-ba8f-77d45382d50b">WSPSend</a> and 
<a href="https://msdn.microsoft.com/5304a5d6-bc99-4a6f-8eeb-668bbd93fc84">WSPRecv</a> can then be used in the same way as a regular service provider.

Every call to 
<b>WPUOpenCurrentThread</b> must have a corresponding call to 
<a href="https://msdn.microsoft.com/1a5e7a99-484f-4862-bd28-edf85debc8e5">WPUCloseThread</a>.




## -see-also




<a href="https://msdn.microsoft.com/1a5e7a99-484f-4862-bd28-edf85debc8e5">WPUCloseThread</a>



<a href="https://msdn.microsoft.com/5304a5d6-bc99-4a6f-8eeb-668bbd93fc84">WSPRecv</a>



<a href="https://msdn.microsoft.com/4d741663-34f5-41b9-ba8f-77d45382d50b">WSPSend</a>
 

 

