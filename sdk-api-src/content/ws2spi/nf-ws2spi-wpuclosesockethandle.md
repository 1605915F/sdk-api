---
UID: NF:ws2spi.WPUCloseSocketHandle
title: WPUCloseSocketHandle function
author: windows-sdk-content
description: The WPUCloseSocketHandle function closes an existing socket handle.
old-location: winsock\wpuclosesockethandle_2.htm
tech.root: WinSock
ms.assetid: c125b763-6c5a-4a83-ba34-79e898fdc9fe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WPUCloseSocketHandle, WPUCloseSocketHandle function [Winsock], _win32_wpuclosesockethandle_2, winsock.wpuclosesockethandle_2, ws2spi/WPUCloseSocketHandle
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
 - WPUCloseSocketHandle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WPUCloseSocketHandle function


## -description


The 
<b>WPUCloseSocketHandle</b> function closes an existing socket handle.


## -parameters




### -param s [in]

Handle to socket created with 
<a href="https://msdn.microsoft.com/ecbf9d8b-b705-4160-ac77-afa5b1501534">WPUCreateSocketHandle</a>.


### -param lpErrno [out]

Pointer to the error code.


## -returns



If no error occurs, 
<a href="https://msdn.microsoft.com/ecbf9d8b-b705-4160-ac77-afa5b1501534">WPUCreateSocketHandle</a> returns zero. Otherwise, it returns SOCKET_ERROR, and a specific error code is available in <i>lpErrno</i>.



<table>
<tr>
<th>Error code</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAENOTSOCK</a></b></dt>
</dl>
</td>
<td width="60%">
The descriptor is not a socket created by 
<a href="https://msdn.microsoft.com/ecbf9d8b-b705-4160-ac77-afa5b1501534">WPUCreateSocketHandle</a>.

</td>
</tr>
</table>
 


<div> </div>





## -remarks



The 
<b>WPUCloseSocketHandle</b> function closes an existing socket handle created by 
<a href="https://msdn.microsoft.com/ecbf9d8b-b705-4160-ac77-afa5b1501534">WPUCreateSocketHandle</a>. This function removes the socket from Ws2_32.dll's internal socket table. The owning service provider is responsible for releasing any resources associated with the socket.




## -see-also




<a href="https://msdn.microsoft.com/ecbf9d8b-b705-4160-ac77-afa5b1501534">WPUCreateSocketHandle</a>
 

 

