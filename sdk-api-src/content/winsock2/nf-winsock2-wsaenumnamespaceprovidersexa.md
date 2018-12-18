---
UID: NF:winsock2.WSAEnumNameSpaceProvidersExA
title: WSAEnumNameSpaceProvidersExA function
author: windows-sdk-content
description: Retrieves information on available namespace providers.
old-location: winsock\wsaenumnamespaceprovidersex.htm
tech.root: winsock
ms.assetid: 34bc96aa-63f7-4ab8-9376-6f4b979225ca
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WSAEnumNameSpaceProvidersEx, WSAEnumNameSpaceProvidersEx function [Winsock], WSAEnumNameSpaceProvidersExA, WSAEnumNameSpaceProvidersExW, winsock.wsaenumnamespaceprovidersex, winsock2/WSAEnumNameSpaceProvidersEx, winsock2/WSAEnumNameSpaceProvidersExA, winsock2/WSAEnumNameSpaceProvidersExW
ms.topic: function
req.header: winsock2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1, Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: WSAEnumNameSpaceProvidersExW (Unicode) and WSAEnumNameSpaceProvidersExA (ANSI)
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
 - WSAEnumNameSpaceProvidersEx
 - WSAEnumNameSpaceProvidersExA
 - WSAEnumNameSpaceProvidersExW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WSAEnumNameSpaceProvidersExA function


## -description


The 
<b>WSAEnumNameSpaceProvidersEx</b> function retrieves information on available namespace providers.


## -parameters




### -param lpdwBufferLength [in, out]

On input, the number of bytes contained in the buffer pointed to by <i>lpnspBuffer</i>. On output (if the function fails, and the error is 
<a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAEFAULT</a>), the minimum number of bytes to allocate for the <i>lpnspBuffer</i> buffer to allow it to retrieve all the requested information. The buffer passed to <b>WSAEnumNameSpaceProvidersEx</b> must be sufficient to hold all of the namespace information.


### -param lpnspBuffer [out]

A buffer that is filled with 
<a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">WSANAMESPACE_INFOEX</a> structures. The returned structures are located consecutively at the head of the buffer. Variable sized information referenced by pointers in the structures point to locations within the buffer located between the end of the fixed sized structures and the end of the buffer. The number of structures filled in is the return value of 
<b>WSAEnumNameSpaceProvidersEx</b>.


## -returns



The 
<b>WSAEnumNameSpaceProvidersEx</b> function returns the number of 
<a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">WSANAMESPACE_INFOEX</a> structures copied into <i>lpnspBuffer</i>. Otherwise, the value SOCKET_ERROR is returned, and a specific error number can be retrieved by calling 
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
The <i>lpnspBuffer</i> parameter was a <b>NULL</b> pointer or the buffer length, <i>lpdwBufferLength</i>, was too small to receive all the relevant 
<a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">WSANAMESPACE_INFOEX</a> structures and associated information. When this error is returned, the buffer length required is returned in the <i>lpdwBufferLength</i> parameter.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSANOTINITIALISED</a></b></dt>
</dl>
</td>
<td width="60%">
The WS2_32.DLL has not been initialized. The application must first call 
<a href="https://msdn.microsoft.com/08299592-867c-491d-9769-d16602133659">WSAStartup</a> before calling any Windows Sockets functions.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSA_NOT_ENOUGH_MEMORY</a></b></dt>
</dl>
</td>
<td width="60%">
There was insufficient memory to perform the operation.

</td>
</tr>
</table>
 




## -remarks



The <b>WSAEnumNameSpaceProvidersEx</b>  function is an enhanced version of the <a href="https://msdn.microsoft.com/f5b6cd42-c5cb-43b6-bb96-fd260217e252">WSAEnumNameSpaceProviders</a> function. The provider-specific data blob associated with the namespace entry
                     passed in the <i>lpProviderInfo</i> parameter to the <a href="https://msdn.microsoft.com/13dde602-c958-4312-a16f-a393dd6fb829">WSCInstallNameSpaceEx</a> function can be queried using <b>WSAEnumNameSpaceProvidersEx</b> function. 

Currently, the only namespace provider included with Windows that sets information in the <b>ProviderSpecific</b> member of the  <a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">WSANAMESPACE_INFOEX</a> structure is the NS_EMAIL provider. The format of the <b>ProviderSpecific</b> member for an NS_EMAIL namespace provider is a <a href="https://msdn.microsoft.com/3444ad63-444a-481d-8fe7-f40b2b7d5283">NAPI_PROVIDER_INSTALLATION_BLOB</a> structure. 

When UNICODE or _UNICODE is defined, <b>WSAEnumNameSpaceProvidersEx</b> is defined to <b>WSAEnumNameSpaceProvidersExW</b>, the Unicode version of this function. The <i>lpnspBuffer</i> parameter is defined to the <a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">LPSAWSANAMESPACE_INFOEXW</a> data type and <b>WSANAMESPACE_INFOEXW</b> structures are returned on success.

When UNICODE or _UNICODE is not defined, <b>WSAEnumNameSpaceProvidersEx</b> is defined to <b>WSAEnumNameSpaceProvidersExA</b>, the ANSI version of this function. The <i>lpnspBuffer</i> parameter is defined to the <a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">LPSAWSANAMESPACE_INFOEXA</a> data type and <b>WSANAMESPACE_INFOEXA</b> structures are returned on success.

<b>Windows 8.1</b> and <b>Windows Server 2012 R2</b>: The  <b>WSAEnumNameSpaceProvidersExW</b> function is supported for Windows Store apps on Windows 8.1, Windows Server 2012 R2, and later.




## -see-also




<a href="https://msdn.microsoft.com/3444ad63-444a-481d-8fe7-f40b2b7d5283">NAPI_PROVIDER_INSTALLATION_BLOB</a>



<a href="https://msdn.microsoft.com/f5b6cd42-c5cb-43b6-bb96-fd260217e252">WSAEnumNameSpaceProviders</a>



<a href="https://msdn.microsoft.com/3f4a8916-9db9-4b65-982f-4cb4ec2205ed">WSANAMESPACE_INFOEX</a>



<a href="https://msdn.microsoft.com/544120b2-7575-4deb-8429-2bd4582eceef">WSCEnumNameSpaceProvidersEx32</a>



<a href="https://msdn.microsoft.com/13dde602-c958-4312-a16f-a393dd6fb829">WSCInstallNameSpaceEx32</a>
 

 

