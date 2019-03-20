---
UID: NF:mprapi.MprAdminServerSetCredentials
title: MprAdminServerSetCredentials function (mprapi.h)
author: windows-sdk-content
description: The MprAdminServerSetCredentials functions sets the pre-shared key for the specified server.
old-location: rras\mpradminserversetcredentials.htm
tech.root: RRAS
ms.assetid: cc77007f-306f-467a-a52f-bf920da15e74
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MprAdminServerSetCredentials, MprAdminServerSetCredentials function [RAS], _mpr_mpradminserversetcredentials, mprapi/MprAdminServerSetCredentials, rras.mpradminserversetcredentials
ms.topic: function
req.header: mprapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.lib: Mprapi.lib
req.dll: Mprapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Mprapi.dll
api_name:
 - MprAdminServerSetCredentials
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MprAdminServerSetCredentials function


## -description


The 
<b>MprAdminServerSetCredentials</b> functions sets the pre-shared key for the specified server.


## -parameters




### -param hMprServer [in]

Handle to a Windows server. Obtain this handle by calling 
<a href="https://msdn.microsoft.com/8d8cba34-e5d3-42ae-9724-361802f21410">MprAdminMIBServerConnect</a>.


### -param dwLevel [in]

A DWORD value that describes the format in which the information is structured in the <i>lpbBuffer</i> parameter. Must be zero.


### -param lpbBuffer [in]

A pointer to an <a href="https://msdn.microsoft.com/b37b9589-5c25-44ac-954a-c9fb2c2ee503">MPR_CREDENTIALSEX_1</a> structure that contains the pre-shared key for the server.


## -returns



If the function succeeds, the return value is NO_ERROR.

If the function fails, the return value is one of the following error codes.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The calling application does not have sufficient privileges.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>lpbBuffer</i> parameter is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The <i>dwLevel</i> parameter is not zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Other</b></dt>
</dl>
</td>
<td width="60%">
Use 
<a href="https://msdn.microsoft.com/b9d61342-4bcf-42e9-96f1-a5993dfb6c0c">FormatMessage</a> to retrieve the system error message that corresponds to the error code returned.

</td>
</tr>
</table>
 




## -remarks



The server maintains a single pre-shared key for all users.

To delete the pre-shared key, call 
<b>MprAdminServerSetCredentials</b> with the <a href="https://msdn.microsoft.com/b37b9589-5c25-44ac-954a-c9fb2c2ee503">MPR_CREDENTIALSEX_1</a><b>dwSize</b> member set to zero.




## -see-also




<a href="https://msdn.microsoft.com/b37b9589-5c25-44ac-954a-c9fb2c2ee503">MPR_CREDENTIALSEX_1</a>



<a href="https://msdn.microsoft.com/76211b14-8f6c-48e4-846f-bd5d3a04285d">MprAdminServerGetCredentials</a>



<a href="https://msdn.microsoft.com/a61734a7-b171-4e38-8dec-46be9a9c08ee">Router Administration Functions</a>



<a href="https://msdn.microsoft.com/352505a9-616a-4d47-9857-f88d345333fd">Router Management Reference</a>
 

 

