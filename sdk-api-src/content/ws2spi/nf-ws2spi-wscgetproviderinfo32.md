---
UID: NF:ws2spi.WSCGetProviderInfo32
title: WSCGetProviderInfo32 function (ws2spi.h)
author: windows-sdk-content
description: Retrieves the data associated with an information class for a 32-bit layered service provider (LSP).Note  This call is a strictly 32-bit version of WSCGetProviderInfo for use on 64-bit platforms.
old-location: winsock\wscgetproviderinfo32.htm
tech.root: WinSock
ms.assetid: 91686b38-3cde-4979-8bf6-45e805dd37ff
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WSCGetProviderInfo32, WSCGetProviderInfo32 function [Winsock], winsock.wscgetproviderinfo32, ws2spi/WSCGetProviderInfo32
ms.topic: function
req.header: ws2spi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - WSCGetProviderInfo32
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WSCGetProviderInfo32 function


## -description


<div class="alert"><b>Note</b>  Layered Service Providers are deprecated. Starting with Windows 8 and Windows Server 2012, use <a href="https://msdn.microsoft.com/0436f559-20e6-4199-8391-10eb7d85df23">Windows Filtering Platform</a>.</div><div> </div>The 
<b>WSCGetProviderInfo32</b> function retrieves the data associated with an information class  for a 32-bit layered service provider (LSP).<div class="alert"><b>Note</b>  This call is a strictly 32-bit version of <a href="https://msdn.microsoft.com/5880f3dd-2a74-4af8-b0d8-2a8eedccc1e6">WSCGetProviderInfo</a> for use on 64-bit platforms. It is provided to allow 64-bit processes to access the 32-bit catalogs.</div>
<div> </div>



## -parameters




### -param lpProviderId [in]

A pointer to a globally unique identifier (GUID)  for the provider. 


### -param InfoType [in]

The information class that is requested for this LSP protocol entry.


### -param Info [out]

A pointer to a buffer to receive the information class data for the requested LSP protocol entry. If this parameter is <b>NULL</b>, then <b>WSCGetProviderInfo32</b> returns failure and the size required for this buffer is returned in the <i>InfoSize</i> parameter.


### -param InfoSize [in, out]

The size, in bytes, of the buffer pointed to by the <i>Info </i>parameter. If the Info parameter is <b>NULL</b>, then  <b>WSCGetProviderInfo32</b> returns failure and the <i>InfoSize</i> parameter will receive the size of the required buffer.


### -param Flags [in]

The flags used to modify the behavior of the <b>WSCGetProviderInfo32</b> function call.


### -param lpErrno [out]

A pointer to the error code if the function fails.


## -returns



If no error occurs, <b>WSCGetProviderInfo32</b> returns <b>ERROR_SUCCESS</b> (zero). Otherwise, it returns <b>SOCKET_ERROR</b>, and a specific error code is returned in the <i>lpErrno</i> parameter.

<table>
<tr>
<th>Error code</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_CALL_NOT_IMPLEMENTED</b></dt>
</dl>
</td>
<td width="60%">
The call is not implemented. This error is returned if <b>ProviderInfoAudit</b> is specified in the <i>InfoType</i> parameter.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAEFAULT</a></b></dt>
</dl>
</td>
<td width="60%">
One or more of the arguments is not in a valid part of the user address space.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAEINVAL</a></b></dt>
</dl>
</td>
<td width="60%">
One or more of the arguments are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSAEINVALIDPROVIDER</a></b></dt>
</dl>
</td>
<td width="60%">
The protocol entry could not be found for the specified <i>lpProviderId</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSANO_RECOVERY</a></b></dt>
</dl>
</td>
<td width="60%">
A nonrecoverable error occurred. This error is returned under several conditions including the following: the user lacks the administrative privileges required to access the Winsock registry, or a failure occurred when opening a Winsock catalog entry.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/en-us/library/ms740668(v=VS.85).aspx">WSA_NOT_ENOUGH_MEMORY</a></b></dt>
</dl>
</td>
<td width="60%">
 Insufficient memory was available. This error is returned when there is insufficient memory to allocate a new catalog entry.

</td>
</tr>
</table>
 




## -remarks



<b>WSCGetProviderInfo32</b> is a strictly 32-bit version of <a href="https://msdn.microsoft.com/5880f3dd-2a74-4af8-b0d8-2a8eedccc1e6">WSCGetProviderInfo</a>. On a 64-bit computer, all calls not specifically 32-bit (for example, all functions that do not end in "32") operate on the native 64-bit catalog. Processes that execute on a 64-bit computer must use the specific 32-bit function calls to operate on a strictly 32-bit catalog and preserve compatibility. The definitions and semantics of the specific 32-bit calls are the same as their native counterparts.

<b>WSCGetProviderInfo32</b> is used to retrieve information class data for a protocol entry on a 32-bit layered service provider. When the <i>InfoType</i> parameter is set to <b>ProviderInfoLspCategories</b>, on success <b>WSCGetProviderInfo32</b> returns with the <i>Info</i> parameter set with appropriate LSP category flags implemented by 32-bit LSP. 

Winsock 2 accommodates layered protocols. A layered protocol is one that implements only higher level communications functions, while relying on an underlying transport stack for the actual exchange of data with a remote endpoint. An example of a layered protocol or layered service provider would be a security layer that adds protocol to the connection establishment process in order to perform authentication and to establish a mutually agreed upon encryption scheme.  Such a security protocol would generally require the services of an underlying reliable transport protocol such as TCP or SPX.  The term base protocol refers to a protocol such as TCP or SPX which is capable of performing data communications with a remote endpoint. The term layered protocol is used to describe a protocol that cannot stand alone.  A protocol chain would then be defined as one or more layered protocols strung together and anchored by a base protocol.
A base protocol has the <b>ChainLen</b> member of the <a href="https://msdn.microsoft.com/758c5553-056f-4ea5-a851-30ef641ffb14">WSAPROTOCOL_INFO</a> structure set to  <b>BASE_PROTOCOL</b> which is defined to be 1. A layered protocol has the <b>ChainLen</b> member of the <b>WSAPROTOCOL_INFO</b> structure set to <b>LAYERED_PROTOCOL</b> which is defined to be zero. A protocol chain has the <b>ChainLen</b> member of the <b>WSAPROTOCOL_INFO</b> structure set to greater than 1.

During LSP initialization, the LSP must provide pointers to a number of Winsock SPI functions.  These functions will be called during normal processing by the layer directly above the LSP (either another LSP or Ws2_32.DLL).  

An LSP that implements an installable file system (IFS) can  selectively choose to provide pointers to functions which are implemented by itself, or pass back the pointers provided by the layer directly below the LSP.  Non-IFS LSPs, because they provide their own handles, must implement all of the Winsock SPI functions.  This is because each SPI will require the LSP to map all of the socket handles it created to the socket handle of the lower provider (either another LSP or the base protocol).

However, all LSPs perform their specific work by doing extra processing on only a subset of the Winsock SPI functions.  

It is possible to define LSP categories based upon the subset of SPI functions an LSP implements and the nature of the extra processing performed for each of those functions.

By classifying LSPs, as well as classifying applications which use Winsock sockets, it becomes possible to selectively determine if an LSP should be involved in a given process at runtime.

On Windows Vista and later, an LSP can be classified based on how it interacts with Windows Sockets calls and data. An LSP category is an identifiable group of behaviors on a subset of Winsock SPI functions.  For example, an HTTP content filter would be categorized as a data inspector (the <b>LSP_INSPECTOR</b> category). The <b>LSP_INSPECTOR</b> category will inspect, but not alter, parameters to data transfer SPI functions. An application can query for the category of an LSP and choose to not load the LSP based on the LSP category and the application's set of permitted LSP categories.

The following table lists categories into which an LSP can be classified.<table>
<tr>
<th>LSP Category</th>
<th>Description</th>
</tr>
<tr>
<td><b>LSP_CRYPTO_COMPRESS</b></td>
<td>The LSP is a cryptography or data compression provider.</td>
</tr>
<tr>
<td><b>LSP_FIREWALL</b></td>
<td>The LSP is a firewall provider.</td>
</tr>
<tr>
<td><b>LSP_LOCAL_CACHE</b></td>
<td>The LSP is a local cache provider.
</td>
</tr>
<tr>
<td><b>LSP_INBOUND_MODIFY</b></td>
<td>The LSP modifies inbound data.</td>
</tr>
<tr>
<td><b>LSP_INSPECTOR</b></td>
<td>The LSP inspects or filters data.
</td>
</tr>
<tr>
<td><b>LSP_OUTBOUND_MODIFY</b></td>
<td>The LSP modifies outbound data.</td>
</tr>
<tr>
<td><b>LSP_PROXY</b></td>
<td>The LSP acts as a proxy and redirects packets.</td>
</tr>
<tr>
<td><b>LSP_REDIRECTOR</b></td>
<td>The LSP is a network redirector.</td>
</tr>
<tr>
<td><b>LSP_SYSTEM</b></td>
<td>The LSP is acceptable for use in services and system processes.</td>
</tr>
</table>
 



An LSP may belong to more than one category.  For example, a firewall/security LSP could belong to both the inspector (<b>LSP_INSPECTOR</b>) and firewall (<b>LSP_FIREWALL</b>) categories.

If an LSP does not have a category set, it is considered to be in the All Other category. This LSP category will not be loaded in services or system processes (for example, lsass, winlogon, and many svchost processes).




## -see-also




<a href="https://msdn.microsoft.com/1c5efd2e-1b42-4c20-a4da-b81a5fc4243c">Categorizing Layered Service Providers and Applications</a>



<a href="https://msdn.microsoft.com/758c5553-056f-4ea5-a851-30ef641ffb14">WSAPROTOCOL_INFO</a>



<a href="https://msdn.microsoft.com/c4e149ce-dff9-401a-8488-23676992c04d">WSCGetApplicationCategory</a>



<a href="https://msdn.microsoft.com/5880f3dd-2a74-4af8-b0d8-2a8eedccc1e6">WSCGetProviderInfo</a>



<a href="https://msdn.microsoft.com/266c9424-f6ab-4630-843d-bc0833d74e4f">WSCSetApplicationCategory</a>



<a href="https://msdn.microsoft.com/adb2737f-5327-4306-bd57-f165f339f911">WSCSetProviderInfo32</a>



<a href="https://msdn.microsoft.com/7f93a660-6f53-4e3c-a938-54a13b34258d">WSC_PROVIDER_INFO_TYPE</a>
 

 

