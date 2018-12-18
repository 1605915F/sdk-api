---
UID: NF:ntsecapi.LsaConnectUntrusted
title: LsaConnectUntrusted function
author: windows-sdk-content
description: Establishes an untrusted connection to the LSA server.
old-location: security\lsaconnectuntrusted.htm
tech.root: secauthn
ms.assetid: b54917c8-51cd-4891-9613-f37a4a46448b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: LsaConnectUntrusted, LsaConnectUntrusted function [Security], _lsa_lsaconnectuntrusted, ntsecapi/LsaConnectUntrusted, security.lsaconnectuntrusted
ms.topic: function
req.header: ntsecapi.h
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
req.lib: Secur32.lib
req.dll: Secur32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Secur32.dll
api_name:
 - LsaConnectUntrusted
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# LsaConnectUntrusted function


## -description


The <b>LsaConnectUntrusted</b> function establishes an untrusted connection to the LSA server.


## -parameters




### -param LsaHandle [out]

Pointer to a handle that receives the connection handle, which must be provided in future authentication services.


## -returns



If the function succeeds, the return value is STATUS_SUCCESS.

If the function fails, the return value is an NTSTATUS code. For more information, see 
<a href="https://msdn.microsoft.com/ee55364e-8ffe-4a78-a49a-250756561770">LSA Policy Function Return Values</a>.

The 
<a href="https://msdn.microsoft.com/fa91794c-c502-4b36-84cc-a8d77c8e9d9f">LsaNtStatusToWinError</a> function converts an NTSTATUS code to a Windows error code.




## -remarks



<b>LsaConnectUntrusted</b> returns a handle to an untrusted connection; it does not verify any information about the caller. The handle should be closed using the 
<a href="https://msdn.microsoft.com/8a956469-9538-4d71-8158-af22aa26f840">LsaDeregisterLogonProcess</a> function.

If your application simply needs to query information from authentication packages, you can use the handle returned by this function in calls to 
<a href="https://msdn.microsoft.com/b891fa60-28b3-4819-9a92-e4524677fa4f">LsaCallAuthenticationPackage</a> and 
<a href="https://msdn.microsoft.com/c6504aea-fdba-44ac-b2dc-070707bb1183">LsaLookupAuthenticationPackage</a>.

Applications with the SeTcbPrivilege privilege may create a trusted connection by calling 
<a href="https://msdn.microsoft.com/1bef2949-b4c8-400e-8a2d-60aa88a4e238">LsaRegisterLogonProcess</a>.




## -see-also




<a href="https://msdn.microsoft.com/b891fa60-28b3-4819-9a92-e4524677fa4f">LsaCallAuthenticationPackage</a>



<a href="https://msdn.microsoft.com/8a956469-9538-4d71-8158-af22aa26f840">LsaDeregisterLogonProcess</a>



<a href="https://msdn.microsoft.com/c6504aea-fdba-44ac-b2dc-070707bb1183">LsaLookupAuthenticationPackage</a>



<a href="https://msdn.microsoft.com/1bef2949-b4c8-400e-8a2d-60aa88a4e238">LsaRegisterLogonProcess</a>
 

 

