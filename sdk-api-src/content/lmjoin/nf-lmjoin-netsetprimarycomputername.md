---
UID: NF:lmjoin.NetSetPrimaryComputerName
title: NetSetPrimaryComputerName function
author: windows-sdk-content
description: Sets the primary computer name for the specified computer.
old-location: netmgmt\netsetprimarycomputername.htm
tech.root: netmgmt
ms.assetid: 524c8219-a303-45ab-95e2-91319b477568
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: NetSetPrimaryComputerName, NetSetPrimaryComputerName function [Network Management], lmjoin/NetSetPrimaryComputerName, netmgmt.netsetprimarycomputername
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: lmjoin.h
req.include-header: Lm.h
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
req.lib: Netapi32.lib
req.dll: Netapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Netapi32.dll
api_name:
 - NetSetPrimaryComputerName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# NetSetPrimaryComputerName function


## -description


The
				<b>NetSetPrimaryComputerName</b> function sets the primary computer name for the specified computer.


## -parameters




### -param Server [in, optional]

A pointer to a constant string that specifies the name of the computer on which to execute this function. If this parameter is <b>NULL</b>, the local computer is used.


### -param PrimaryName [in]

A pointer to a constant string that specifies the primary name to set. This name must be in the form of a fully qualified DNS name.


### -param DomainAccount [in, optional]

A pointer to a constant string that specifies the domain account to use for accessing the
        machine account object for the computer specified in the <i>Server</i> parameter in Active Directory. If this parameter is <b>NULL</b>, then the credentials of the user executing
        this routine are used. 

This parameter is not used if the server to execute this function is not joined to a domain. 


### -param DomainAccountPassword [in, optional]

A pointer to a constant string that specifies the password matching the domain account passed in the <i>DomainAccount</i> parameter.
        If this parameter is <b>NULL</b>, then the credentials of the user executing
        this routine are used. 

This parameter is ignored if the <i>DomainAccount</i> parameter is <b>NULL</b>. This parameter is not used if the server to execute this function is not joined to a domain. 


### -param Reserved [in]

Reserved for future use.   This parameter should be <b>NULL</b>.


## -returns



If the function succeeds, the return value is NERR_Success.

If the function fails, the return value can be one of the following error codes or one of the 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
Access is denied. This error is returned if the caller was not a member of the Administrators local group on the target computer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_NAME</b></dt>
</dl>
</td>
<td width="60%">
A name parameter is incorrect. This error is returned if the <i>PrimaryName</i> parameter does not contain valid name.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
A parameter is incorrect. This error is returned if the <i>DomainAccount</i> parameter does not contain a valid domain. This error is also returned if the <i>DomainAccount</i> parameter is not <b>NULL</b> and the <i>DomainAccountPassword</i> parameter is not <b>NULL</b> but does not contain a Unicode string.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Not enough memory is available to process this command.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The request is not supported. This error is returned if the target computer specified in the <i>Server</i> parameter on which this function executes is running on Windows 2000 and earlier. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>NERR_WkstaNotStarted</b></dt>
</dl>
</td>
<td width="60%">
The Workstation service has not been started.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_CALL_IN_PROGRESS</b></dt>
</dl>
</td>
<td width="60%">
A remote procedure call is already in progress for this thread.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_PROTSEQ_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The remote procedure call protocol sequence is not supported.

</td>
</tr>
</table>
 




## -remarks



The <b>NetSetPrimaryComputerName</b> function is supported on Windows XP and later.  

The <b>NetSetPrimaryComputerName</b> function is used as part of computer rename operations. The specified name will be removed from the alternate name list configured for the target computer and configured as the primary name. The computer account name will be changed to match the primary name. The previous primary computer name is moved to the alternate computer name list configured for the computer.

The <b>NetSetPrimaryComputerName</b> function requires that the caller is a member of the Administrators local group on the target computer.




## -see-also




<a href="https://msdn.microsoft.com/710865c6-e327-439c-931d-de8674d69233">NetAddAlternateComputerName</a>



<a href="https://msdn.microsoft.com/c657ae33-404e-4c36-a956-5fbcfa540be7">NetEnumerateComputerNames</a>



<a href="https://msdn.microsoft.com/4efcb399-03af-4312-9f1d-6bc38f356cac">NetJoinDomain</a>



<a href="https://msdn.microsoft.com/3c7ab44e-d5fa-40da-83fe-a44bf85b2ba5">NetRemoveAlternateComputerName</a>



<a href="https://msdn.microsoft.com/1f7ddaa1-a349-49a6-856d-a2fde2f1dc3b">NetRenameMachineInDomain</a>



<a href="https://msdn.microsoft.com/cc755c22-1fd6-4787-999e-a43258287a05">NetUnjoinDomain</a>



<a href="https://msdn.microsoft.com/12163456-770c-4f9e-9261-a6ea5f2cd93a">SetComputerNameEx</a>
 

 

