---
UID: NF:mprapi.MprAdminTransportSetInfo
title: MprAdminTransportSetInfo function (mprapi.h)
author: windows-sdk-content
description: The MprAdminTransportSetInfo function sets global information, or default client interface information, or both, for a specified transport.
old-location: rras\mpradmintransportsetinfo.htm
tech.root: RRAS
ms.assetid: ac0be570-e484-481b-9b16-ccdd4870deda
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MprAdminTransportSetInfo, MprAdminTransportSetInfo function [RAS], _mpr_mpradmintransportsetinfo, mprapi/MprAdminTransportSetInfo, rras.mpradmintransportsetinfo
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
 - MprAdminTransportSetInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MprAdminTransportSetInfo function


## -description


The 
<b>MprAdminTransportSetInfo</b> function sets global information, or default client interface information, or both, for a specified transport.


## -parameters




### -param hMprServer [in]

Handle to the router on which information is being set. This handle is obtained from a previous call to 
<a href="https://msdn.microsoft.com/f93b37bc-d3d1-40f0-aef6-839bb43c88e2">MprAdminServerConnect</a>.


### -param dwTransportId [in]

A <b>DWORD</b> value that describes the transport type to set. Acceptable values for <i>dwTransportId</i> are listed in the following table.

<table>
<tr>
<th>Value</th>
<th>Transport (Protocol Family)</th>
</tr>
<tr>
<td>PID_ATALK</td>
<td>AppleTalk</td>
</tr>
<tr>
<td>PID_IP</td>
<td>Internet Protocol version 4</td>
</tr>
<tr>
<td>PID_IPX</td>
<td>Internet Packet Exchange</td>
</tr>
<tr>
<td>PID_NBF</td>
<td>NetBIOS Frames Protocol</td>
</tr>
<tr>
<td>PID_IPV6</td>
<td>Windows Server 2008 or later: Internet Protocol version 6</td>
</tr>
</table>
 


### -param pGlobalInfo [in, optional]

Pointer to a buffer that specifies global information for the transport. Use the 
<a href="https://msdn.microsoft.com/e88720aa-080b-4d87-a442-1b436c256ca6">Information Header Functions</a> to manipulate information headers. 




This parameter is optional. If the calling application specifies <b>NULL</b> for this parameter, the function does not set the global information.


### -param dwGlobalInfoSize [in]

Specifies the size, in bytes, of the buffer pointed to by the <i>pGlobalInfo</i> parameter.


### -param pClientInterfaceInfo [in, optional]

Pointer to a buffer that specifies default client interface information for the transport. 




This parameter is optional. If the calling application specifies <b>NULL</b> for this parameter, the function does not set the default client interface information.


### -param dwClientInterfaceInfoSize [in]

Specifies the size, in bytes, of the buffer pointed to by the <i>pClientInterfaceInfo</i> parameter.


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
The <i>pGlobalInfo</i> parameter and the <i>pClientInterfaceInfo</i> parameter are both <b>NULL</b>.

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
<dt><b>ERROR_UNKNOWN_PROTOCOL_ID</b></dt>
</dl>
</td>
<td width="60%">
The <i>dwTransportId</i> value does not match any supported transport protocols.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/f93b37bc-d3d1-40f0-aef6-839bb43c88e2">MprAdminServerConnect</a>



<a href="https://msdn.microsoft.com/47fbe483-8a1b-4747-9555-931dd63e2db8">MprAdminTransportGetInfo</a>



<a href="https://msdn.microsoft.com/a61734a7-b171-4e38-8dec-46be9a9c08ee">Router Administration Functions</a>



<a href="https://msdn.microsoft.com/352505a9-616a-4d47-9857-f88d345333fd">Router Management Reference</a>
 

 

