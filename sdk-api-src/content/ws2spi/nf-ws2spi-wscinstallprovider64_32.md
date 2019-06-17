---
UID: NF:ws2spi.WSCInstallProvider64_32
title: WSCInstallProvider64_32 function (ws2spi.h)
author: windows-sdk-content
description: Installs the specified transport service provider into the 32-bit and 64-bit system configuration databases on a 64-bit computer.
old-location: winsock\wscinstallprovider64_32.htm
tech.root: WinSock
ms.assetid: 50d3a5d1-18f2-439e-a16c-6f31becb1e65
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WSCInstallProvider64_32, WSCInstallProvider64_32 function [Winsock], winsock.wscinstallprovider64_32, ws2spi/WSCInstallProvider64_32
ms.topic: function
f1_keywords: ["ws2spi/WSCInstallProvider64_32"]
req.header: ws2spi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Professional x64 Edition [desktop apps only]
req.target-min-winversvr: Windows Server 2003 x64 Edition [desktop apps only]
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
 - WSCInstallProvider64_32
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# WSCInstallProvider64_32 function


## -description


<p class="CCE_Message">[<b>WSCInstallProvider64_32</b> is no longer available for use as of Windows Vista. Instead, use <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallprovider">WSCInstallProvider</a> or <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallproviderandchains">WSCInstallProviderAndChains</a>.]

The <b>WSCInstallProvider64_32</b> function installs the specified transport service provider into the 32-bit and 64-bit system configuration databases on a 64-bit computer.


## -parameters




### -param lpProviderId [in]

A pointer to a globally unique identifier (GUID)  for the provider.


### -param lpszProviderDllPath [in]

A pointer to a Unicode string that contains the load path to the provider 64-bit DLL. This string observes the usual rules for path resolution and can contain embedded environment strings (such as %SystemRoot%). Such environment strings are expanded when the Ws2_32.dll must subsequently load the provider DLL on behalf of an application. After any embedded environment strings are expanded, the Ws2_32.dll passes the resulting string to the <a href="https://docs.microsoft.com/windows/desktop/api/libloaderapi/nf-libloaderapi-loadlibrarya">LoadLibrary</a> function which loads the provider into memory. For more information, see <b>LoadLibrary</b>.


### -param lpProtocolInfoList [in]

A pointer to an array of 
<a href="https://docs.microsoft.com/windows/desktop/api/winsock2/ns-winsock2-_wsaprotocol_infoa">WSAPROTOCOL_INFO</a> structures. Each structure defines a protocol, address family, and socket type supported by the provider.


### -param dwNumberOfEntries [in]

The number of entries in the <i>lpProtocolInfoList</i> array.


### -param lpErrno [out]

A pointer to the error code if the function fails.


## -returns



If <b>WSCInstallProvider64_32</b> succeeds, it returns zero. Otherwise, it returns <b>SOCKET_ERROR</b>, and a specific error code is returned in the <i>lpErrno</i> parameter.

<table>
<tr>
<th>Error code</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSAEFAULT</a></b></dt>
</dl>
</td>
<td width="60%">
One or more of the arguments is not in a valid part of the user address space.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSAEINVAL</a></b></dt>
</dl>
</td>
<td width="60%">
One or more of the arguments are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSAENOBUFS</a></b></dt>
</dl>
</td>
<td width="60%">
 Memory could not be allocated for buffers.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSANO_RECOVERY</a></b></dt>
</dl>
</td>
<td width="60%">
A nonrecoverable error occurred. This error is returned under several conditions including the following: the provider is already installed, the user lacks the administrative privileges required to write to the  Winsock registry, or a failure occurred when creating or installing a catalog entry.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSASYSCALLFAILURE</a></b></dt>
</dl>
</td>
<td width="60%">
 A system call that should never fail has failed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSA_NOT_ENOUGH_MEMORY</a></b></dt>
</dl>
</td>
<td width="60%">
 Insufficient memory was available. This error is returned when there is insufficient memory to allocate a new catalog entry.

</td>
</tr>
</table>
 




## -remarks



<b>WSCInstallProvider64_32</b> is a basic version of the <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallproviderandchains64_32">WSCInstallProviderAndChains64_32</a> function that only installs a single transport service provider. <b>WSCInstallProvider64_32</b> can be used to install a base protocol, a layered protocol, or a protocol chain. If a layered service provider is being installed, then <b>WSCInstallProviderAndChains64_32</b> should be used because this function allows a layered protocol and one or more protocol chains to be installed with a single function call. To accomplish the same work using <b>WSCInstallProvider64_32</b> would require multiple function calls to install each service provider component.

Windows Sockets (Winsock) 2 accommodates the notion of a layered protocol. A layered protocol is one that implements only higher level communications functions while relying on an underlying transport stack for the actual exchange of data with a remote endpoint. An example of a layered protocol would be a security layer that adds  a protocol to the connection establishment process to perform authentication and to establish a mutually agreed upon encryption scheme.  Such a security protocol would generally require the services of an underlying reliable transport protocol such as TCP or SPX.  The term base protocol refers to a protocol such as TCP or SPX which is fully capable of performing data communications with a remote endpoint. The term layered protocol is used to describe a protocol that cannot stand alone.  A protocol chain would then be defined as one or more layered protocols strung together and anchored by a base protocol.
A base protocol has the <b>ChainLen</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/winsock2/ns-winsock2-_wsaprotocol_infoa">WSAPROTOCOL_INFO</a> structure set to  <b>BASE_PROTOCOL</b> which is defined to be 1. A layered protocol has the <b>ChainLen</b> member of the <b>WSAPROTOCOL_INFO</b> structure set to <b>LAYERED_PROTOCOL</b> which is defined to be zero. A protocol chain has the <b>ChainLen</b> member of the <b>WSAPROTOCOL_INFO</b> structure set to greater than 1.

<b>WSCInstallProvider64_32</b> is the 64-bit version of <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallprovider">WSCInstallProvider</a> that installs the provider into both the 32-bit and 64-bit catalogs on 64-bit platforms. That is, on 64-bit platforms, two Winsock catalogs are maintained, and both 32-bit and 64-bit processes are able to load the transport provider installed with this function. On 64-bit platforms, <b>WSCInstallProvider</b> installs only to the 64-bit Winsock catalog.

On a 64-bit computer, all calls not specifically designed for 32-bit (for example, all functions that do not end in "32") operate on the native 64-bit catalog. Processes that execute on a 64-bit computer must use <b>WSCInstallProvider64_32</b> to operate on both the 32-bit catalog as well as the 64-bit catalog, preserving compatibility. The definitions and semantics of the specific 32-bit calls are the same as their native counterparts.

This routine creates the necessary common Winsock 2 configuration information for the specified provider. It is applicable to base protocols, layered protocols, and protocol chains.

The <i>lpProtocolInfoList</i> parameter contains a list of protocol entries to install. Callers of <b>WSCInstallProvider64_32</b>  are responsible for setting up the proper protocol entries. The <i>lpProtocolInfoList</i> parameter must not be <b>NULL</b>. 

After this routine completes successfully, the protocol information provided in <i>lpProtocolInfoList</i> will be returned by <a href="https://docs.microsoft.com/windows/desktop/api/winsock2/nf-winsock2-wsaenumprotocolsa">WSAEnumProtocols</a>, <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscenumprotocols">WSCEnumProtocols</a>, or <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscenumprotocols32">WSCEnumProtocols32</a>. Be aware that in Windows, only instances of the Ws2_32.dll created by calling <a href="https://docs.microsoft.com/windows/desktop/api/winsock/nf-winsock-wsastartup">WSAStartup</a> after a successful completion of this function will include the new entries in 
<b>WSAEnumProtocols</b>, <b>WSCEnumProtocols</b>, and <b>WSCEnumProtocols32</b>. <div class="alert"><b>Note</b>   The <a href="https://docs.microsoft.com/windows/desktop/api/winsock2/nf-winsock2-wsaenumprotocolsa">WSAEnumProtocols</a> function does not enumerate a layered protocol entry while <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscenumprotocols">WSCEnumProtocols</a> and <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscenumprotocols32">WSCEnumProtocols32</a> do.</div>
<div> </div>


On success, <b>WSCInstallProvider64_32</b> will attempt to alert all interested applications that have registered for notification of the change by calling <a href="https://docs.microsoft.com/windows/desktop/api/winsock2/nf-winsock2-wsaproviderconfigchange">WSAProviderConfigChange</a>.

The <b>WSCInstallProvider64_32</b> function can only be called by a user logged on as a member of the Administrators group. If <b>WSCInstallProvider64_32</b> is called by a user that is not a member of the Administrators group, the function call will fail and <a href="https://docs.microsoft.com/windows/desktop/WinSock/windows-sockets-error-codes-2">WSANO_RECOVERY</a> is returned in the <i>lpErrno</i> parameter. 
 For computers running Windows Vista or Windows Server 2008, this function can also fail because of user account control (UAC). If an application  that contains this function is executed by a user logged on as a member of the Administrators group other than the built-in Administrator, this call will fail unless the application has been marked in the manifest file with a <b>requestedExecutionLevel</b> set to <b>requireAdministrator</b>. If the application on Windows Vista or Windows Server 2008 lacks this manifest file, a user logged on as a member of the Administrators group other than the built-in Administrator must then be executing the application in an enhanced shell as the built-in Administrator (<b>RunAs administrator</b>) for this function to succeed.



Any file installation or service provider-specific configuration must be performed by the calling application.

If the <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallprovider">WSCInstallProvider</a> or <a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallproviderandchains">WSCInstallProviderAndChains</a> function is used, the function must be called once to install the provider in the 32-bit catalog and once to install the provider in the 64-bit catalog on a 64-bit platform.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/libloaderapi/nf-libloaderapi-loadlibrarya">LoadLibrary</a>



<a href="https://docs.microsoft.com/windows/desktop/WinSock/transport-configuration-and-installation-2">Transport Configuration and Installation</a>



<a href="https://docs.microsoft.com/windows/desktop/WinSock/transport-service-providers-2">Transport Service Providers</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winsock2/nf-winsock2-wsaenumprotocolsa">WSAEnumProtocols</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winsock2/nf-winsock2-wsaproviderconfigchange">WSAProviderConfigChange</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winsock/nf-winsock-wsastartup">WSAStartup</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscdeinstallprovider32">WSCDeinstallProvider32</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscenumprotocols">WSCEnumProtocols</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscenumprotocols32">WSCEnumProtocols32</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallprovider">WSCInstallProvider</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallproviderandchains">WSCInstallProviderAndChains</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wscinstallproviderandchains64_32">WSCInstallProviderAndChains64_32</a>
 

 

