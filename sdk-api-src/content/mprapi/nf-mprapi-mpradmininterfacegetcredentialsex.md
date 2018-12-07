---
UID: NF:mprapi.MprAdminInterfaceGetCredentialsEx
title: MprAdminInterfaceGetCredentialsEx function
author: windows-sdk-content
description: Use the MprAdminInterfaceGetCredentialsEx function to retrieve extended credentials information for the specified interface. Use this function to retrieve credentials information used for Extensible Authentication Protocols (EAPs).
old-location: rras\mpradmininterfacegetcredentialsex.htm
tech.root: rras
ms.assetid: 0ef9f437-a15b-4f6c-ac76-4c31a23e8792
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MprAdminInterfaceGetCredentialsEx, MprAdminInterfaceGetCredentialsEx function [RAS], _mpr_mpradmininterfacegetcredentialsex, mprapi/MprAdminInterfaceGetCredentialsEx, rras.mpradmininterfacegetcredentialsex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: mprapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
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
 - MprAdminInterfaceGetCredentialsEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MprAdminInterfaceGetCredentialsEx function


## -description


Use the 
<b>MprAdminInterfaceGetCredentialsEx</b> function to retrieve extended credentials information for the specified interface. Use this function to retrieve credentials information used for Extensible Authentication Protocols (EAPs).


## -parameters




### -param hMprServer [in]

Handle to a router. This handle is obtained from a previous call to 
<a href="https://msdn.microsoft.com/f93b37bc-d3d1-40f0-aef6-839bb43c88e2">MprAdminServerConnect</a>. 


### -param hInterface [in]

Handle to the interface. This handle is obtained from a previous call to 
<a href="https://msdn.microsoft.com/c9590ebe-7e49-4ad1-bd9b-0d9c51938bc4">MprAdminInterfaceCreate</a>.


### -param dwLevel [in]

A DWORD value that describes the format in which the information is returned in the <i>lplpbBuffer</i> parameter. Acceptable values for <i>dwLevel</i> include 0 or 1, as listed in the following table. 

<table>
<tr>
<th>Value</th>
<th>Structure Format</th>
</tr>
<tr>
<td>0</td>
<td>Windows 2000 Server: <a href="https://msdn.microsoft.com/a1524c6e-3a94-4fc1-be28-bcaca8bcc62e">MPR_CREDENTIALSEX_0</a>
</td>
</tr>
<tr>
<td>1</td>
<td>Windows Server 2003 or later: <a href="https://msdn.microsoft.com/b37b9589-5c25-44ac-954a-c9fb2c2ee503">MPR_CREDENTIALSEX_1</a>
</td>
</tr>
</table>
 

A value of 1 indicates the information is a pre-shared key for the interface, which is in an encrypted format. 


### -param lplpbBuffer [out]

On successful completion, a pointer to a 
<a href="https://msdn.microsoft.com/a1524c6e-3a94-4fc1-be28-bcaca8bcc62e">MPR_CREDENTIALSEX_0</a> or <a href="https://msdn.microsoft.com/b37b9589-5c25-44ac-954a-c9fb2c2ee503">MPR_CREDENTIALSEX_1</a> structure. The <i>dwLevel</i> parameter indicates the type of structure.
					Free the memory occupied by this structure with 
<a href="https://msdn.microsoft.com/60cae055-841a-4435-bf0e-4198b1ccdd4e">MprAdminBufferFree</a>.


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
<dt><b>ERROR_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
The <i>hInterface</i> value is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>lplpbBuffer</i> parameter is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient resources to complete the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The <i>dwLevel</i> value is invalid.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/a1524c6e-3a94-4fc1-be28-bcaca8bcc62e">MPR_CREDENTIALSEX_0</a>



<a href="https://msdn.microsoft.com/b37b9589-5c25-44ac-954a-c9fb2c2ee503">MPR_CREDENTIALSEX_1</a>



<a href="https://msdn.microsoft.com/c9590ebe-7e49-4ad1-bd9b-0d9c51938bc4">MprAdminInterfaceCreate</a>



<a href="https://msdn.microsoft.com/0ec18926-1ee9-4e28-9284-9d95d06be2e4">MprAdminInterfaceGetCredentials</a>



<a href="https://msdn.microsoft.com/d0807c03-3994-4624-97ea-94b55e7cd1e4">MprAdminInterfaceSetCredentialsEx</a>



<a href="https://msdn.microsoft.com/f93b37bc-d3d1-40f0-aef6-839bb43c88e2">MprAdminServerConnect</a>
 

 

