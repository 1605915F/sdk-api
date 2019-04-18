---
UID: NF:winsock2.gethostname
title: gethostname function (winsock2.h)
author: windows-sdk-content
description: The gethostname function retrieves the standard host name for the local computer.
old-location: winsock\gethostname_2.htm
tech.root: WinSock
ms.assetid: 8fa40b60-0e93-493b-aee1-cea6cf595707
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "_win32_gethostname_2, gethostname, gethostname function [Winsock], winsock.gethostname_2, winsock/gethostname"
ms.topic: function
req.header: winsock2.h
req.include-header: Winsock2.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1, Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Ws2_32.lib
req.dll: Ws2_32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ws2_32.dll
api_name:
 - gethostname
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# gethostname function


## -description


The 
<b>gethostname</b> function retrieves the standard host name for the local computer.


## -parameters




### -param name [out]

A pointer to a buffer that receives the local host name.


### -param namelen [in]

The length, in bytes, of the buffer pointed to by the <i>name</i> parameter.


## -returns



If no error occurs, 
<b>gethostname</b> returns zero. Otherwise, it returns SOCKET_ERROR and a specific error code can be retrieved by calling 
<a href="https://msdn.microsoft.com/39e41b66-44ed-46dc-bfc2-65228b669992">WSAGetLastError</a>.

<table>
<tr>
<th>Error code</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAEFAULT</a></b></dt>
</dl>
</td>
<td width="60%">
The <i>name</i> parameter is a <b>NULL</b> pointer or is not a valid part of the user address space. This error is also returned if the buffer size specified by <i>namelen</i> parameter is too small to hold the complete host name.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSANOTINITIALISED</a></b></dt>
</dl>
</td>
<td width="60%">
A successful 
<a href="https://msdn.microsoft.com/08299592-867c-491d-9769-d16602133659">WSAStartup</a> call must occur before using this function.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAENETDOWN</a></b></dt>
</dl>
</td>
<td width="60%">
The network subsystem has failed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAEINPROGRESS</a></b></dt>
</dl>
</td>
<td width="60%">
A blocking Windows Sockets 1.1 call is in progress, or the service provider is still processing a callback function.

</td>
</tr>
</table>
 




## -remarks



The 
<b>gethostname</b> function returns the name of the local host into the buffer specified by the <i>name</i> parameter. The host name is returned as a <b>null</b>-terminated string. The form of the host name is dependent on the Windows Sockets provider—it can be a simple host name, or it can be a fully qualified domain name. However, it is guaranteed that the name returned will be successfully parsed by 
<a href="https://msdn.microsoft.com/2526ecb5-927b-40c8-8d8f-919e7986ff05">gethostbyname</a> and 
<a href="https://msdn.microsoft.com/1a2b9c76-6e84-4ac2-b5c1-a2268edd0c49">WSAAsyncGetHostByName</a>.

The maximum length of the name returned in the buffer pointed to by the <i>name</i> parameter is dependent on the namespace provider.

If the 
<b>gethostname</b> function is used on a cluster resource on Windows Server 2008, Windows Server 2003, or 
  Windows 2000 Server and the _CLUSTER_NETWORK_NAME_ environment variable is defined, then the value in this environment variable overrides the actual hostname and is returned. On a cluster resource, the _CLUSTER_NETWORK_NAME_ environment variable contains the name of the cluster.

The 
<b>gethostname</b> function queries namespace providers to determine the local host name using the SVCID_HOSTNAME GUID defined in the <i>Svgguid.h</i> header file. If no namespace provider responds, then the 
<b>gethostname</b> function returns the NetBIOS name of the local computer.

The maximum length, in bytes, of the string returned in the buffer pointed to by the <i>name</i> parameter is dependent on the namespace provider, but this string must be 256 bytes or less. So if a buffer of 256 bytes is passed in the <i>name</i> parameter and the <i>namelen</i> parameter is set to 256, the buffer size will always be adequate.


<div class="alert"><b>Note</b>  If no local host name has been configured, 
<b>gethostname</b> must succeed and return a token host name that 
<a href="https://msdn.microsoft.com/2526ecb5-927b-40c8-8d8f-919e7986ff05">gethostbyname</a> or 
<a href="https://msdn.microsoft.com/1a2b9c76-6e84-4ac2-b5c1-a2268edd0c49">WSAAsyncGetHostByName</a> can resolve.</div>
<div> </div>


<b>Windows Phone 8:</b> This function is supported for Windows Phone Store apps on Windows Phone 8 and later.

<b>Windows 8.1</b> and <b>Windows Server 2012 R2</b>: This function is supported for Windows Store apps on Windows 8.1, Windows Server 2012 R2, and later.




## -see-also




<a href="https://msdn.microsoft.com/82436a88-5b37-4758-a5c9-b60dd1cbc36c">GetAddrInfoW</a>



<a href="https://msdn.microsoft.com/1a2b9c76-6e84-4ac2-b5c1-a2268edd0c49">WSAAsyncGetHostByName</a>



<a href="https://msdn.microsoft.com/edafb5f9-09fe-4f8e-9651-4002b6f622f4">Winsock Functions</a>



<a href="https://msdn.microsoft.com/baae2bf9-f505-4365-b60e-e3247a0218c8">Winsock Reference</a>



<a href="https://msdn.microsoft.com/2526ecb5-927b-40c8-8d8f-919e7986ff05">gethostbyname</a>
 

 

