---
UID: NF:iphlpapi.SetPerTcpConnectionEStats
title: SetPerTcpConnectionEStats function (iphlpapi.h)
author: windows-sdk-content
description: Sets a value in the read/write information for an IPv4 TCP connection. This function is used to enable or disable extended statistics for an IPv4 TCP connection.
old-location: iphlp\setpertcpconnectionestats.htm
tech.root: IpHlp
ms.assetid: 96d838ca-69e3-4a73-b969-3e6e810a0a69
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetPerTcpConnectionEStats, SetPerTcpConnectionEStats function [IP Helper], iphlp.setpertcpconnectionestats, iphlpapi/SetPerTcpConnectionEStats
ms.topic: function
req.header: iphlpapi.h
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
req.lib: Iphlpapi.lib
req.dll: Iphlpapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Iphlpapi.dll
api_name:
 - SetPerTcpConnectionEStats
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetPerTcpConnectionEStats function


## -description


The 
<b>SetPerTcpConnectionEStats</b> function  sets a value in the read/write information for an IPv4 TCP connection. This function is used to enable or disable extended statistics for an IPv4 TCP connection.


## -parameters




### -param Row

A pointer to a <a href="https://msdn.microsoft.com/36364854-caa8-4652-be8e-f741b36d9fd7">MIB_TCPROW</a> structure for an IPv4 TCP connection. 


### -param EstatsType

The type of extended statistics for TCP to set. This parameter determines the data and format of information that is expected in the <i>Rw</i> parameter.

This parameter can be one of the values from the <a href="https://msdn.microsoft.com/96f55528-e74a-4360-a7a2-54ba19c3a284">TCP_ESTATS_TYPE</a> enumeration type defined in the <i>Tcpestats.h</i> header file. 


### -param Rw

A pointer to a buffer that contains the read/write information to set. The buffer should contain a value from the <a href="https://msdn.microsoft.com/68f8f797-06fb-4286-88bc-220c54977575">TCP_BOOLEAN_OPTIONAL</a> enumeration for each structure member that specifies how each member should be updated. 


### -param RwVersion

The version of the read/write information to be set. This parameter should be set to zero for Windows Vista, Windows Server 2008, and Windows 7.


### -param RwSize

The size, in bytes, of the buffer pointed to by the <i>Rw</i> parameter.


### -param Offset

The offset, in bytes, to the member in the structure pointed to by the <i>Rw</i> parameter to be set. This parameter is currently unused and must be set to zero.


## -returns



If the function succeeds, the return value is NO_ERROR.

If the function fails, the return value is one of the following error codes.

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
Access is denied. This error is returned under several conditions that include the following: the  user lacks the required administrative privileges on the local computer or the application is not running in an enhanced shell as the built-in Administrator (RunAs administrator).  

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_USER_BUFFER</b></dt>
</dl>
</td>
<td width="60%">
The supplied user buffer is not valid for the requested operation. This error is returned if the <i>Row</i> parameter is a <b>NULL</b> pointer and the <i>RwSize</i> parameter is nonzero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The parameter is incorrect. This error is returned if the <i>Row</i> parameter is a <b>NULL</b> pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
This requested entry was not found. This error is returned if the TCP connection specified in the <i>Row</i> parameter could not be found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The request is not supported. This error is returned if the <i>RwVersion</i> or the <i>Offset</i> parameter is not set to 0.

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
<a href="https://msdn.microsoft.com/b9d61342-4bcf-42e9-96f1-a5993dfb6c0c">FormatMessage</a> to obtain the message string for the returned error.

</td>
</tr>
</table>
 




## -remarks



The <b>SetPerTcpConnectionEStats</b> function is defined on Windows Vista and later. 

The <b>SetPerTcpConnectionEStats</b> function is used to enable or disable extended statistics on an IPv4 TCP connection passed in the <i>Row</i> parameter. Extended statistics on a TCP connection are disabled by default. The <b>SetPerTcpConnectionEStats</b> function is used to set the value of a member in the read/write information for extended statistics for an IPv4 TCP connection. The type and format of the structure to be set is specified by the <i>EstatsType</i> parameter. The <i>Rw</i> parameter contains a pointer to the structure being passed.  All members in the structure pointed to by <i>Rw</i> parameter must be specified. 

The only version of TCP connection statistics currently supported is version zero. So the <i>RwVersion</i> parameter passed to <b>SetPerTcpConnectionEStats</b> should be set to 0.

The structure pointed to by the <i>Rw</i> parameter passed this function depends on the enumeration value passed in the <i>EstatsType</i> parameter. The following table below indicates the structure type that should be passed in the <i>Rw</i> parameter for each possible <i>EstatsType</i> parameter type.  


<table>
<tr>
<th><i>EstatsType</i></th>
<th>Structure pointed to by <i>Rw</i></th>
</tr>
<tr>
<td><b>TcpConnectionEstatsData</b></td>
<td>
<a href="https://msdn.microsoft.com/823cea66-f719-40f6-82bd-572623188446">TCP_ESTATS_DATA_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsSndCong</b></td>
<td>
<a href="https://msdn.microsoft.com/7fc7fb6a-4486-450f-b60e-8cf07b33c79a">TCP_ESTATS_SND_CONG_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsPath</b></td>
<td>
<a href="https://msdn.microsoft.com/460ad710-06aa-490a-9bac-5a8c731687e9">TCP_ESTATS_PATH_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsSendBuff</b></td>
<td>
<a href="https://msdn.microsoft.com/1bc88d95-24d2-4ca3-9f4a-298d5c08f4de">TCP_ESTATS_SEND_BUFF_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsRec</b></td>
<td>
<a href="https://msdn.microsoft.com/e780ae7b-30c6-4890-8a8b-9e0b2739c176">TCP_ESTATS_REC_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsObsRec</b></td>
<td>
<a href="https://msdn.microsoft.com/91c2d5d9-3198-42a7-abf7-077281b491f2">TCP_ESTATS_OBS_REC_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsBandwidth</b></td>
<td>
<a href="https://msdn.microsoft.com/a9bf5ad3-a8db-4194-8e47-5a7409391f4c">TCP_ESTATS_BANDWIDTH_RW_v0</a>
</td>
</tr>
<tr>
<td><b>TcpConnectionEstatsFineRtt</b></td>
<td>
<a href="https://msdn.microsoft.com/35834c9a-2896-4c11-aef7-c55af7f6fef3">TCP_ESTATS_FINE_RTT_RW_v0</a>
</td>
</tr>
</table>
 



The <i>Offset</i> parameter is currently unused and must be set to 0. The possible structures pointed to by the <i>Rw</i> parameter all have a single member except for the <a href="https://msdn.microsoft.com/a9bf5ad3-a8db-4194-8e47-5a7409391f4c">TCP_ESTATS_BANDWIDTH_RW_v0</a> structure.  When the <i>EstatsType</i> parameter is set to <b>TcpConnectionEstatsBandwidth</b>, the <b>TCP_ESTATS_BANDWIDTH_RW_v0</b> structure pointed to by the <i>Rw</i> parameter must have both structure members set  to the preferred values in a single call to the  <b>SetPerTcpConnectionEStats</b> function.

If the <i>RwSize</i> parameter is set to 0, the <b>SetPerTcpConnectionEStats</b> function  returns NO_ERROR and makes no changes tothe extended statistics status.

The <a href="https://msdn.microsoft.com/e90c5aa0-3126-489b-af44-bf86cb45a6d1">GetTcpTable</a> function is used to retrieve the IPv4 TCP connection table on the local computer. This function returns a <a href="https://msdn.microsoft.com/a8ed8ac2-a72f-4099-ac99-a8b0b77b7b84">MIB_TCPTABLE</a> structure that contain an array of <a href="https://msdn.microsoft.com/36364854-caa8-4652-be8e-f741b36d9fd7">MIB_TCPROW</a> entries. The <i>Row</i> parameter passed to the <b>SetPerTcpConnectionEStats</b> function must be an entry for an existing IPv4 TCP connection.

Once extended statistics are enabled on a TCP connection for IPv4, applications call the <a href="https://msdn.microsoft.com/71b9d795-6050-4a1a-9949-2c970801f52c">GetPerTcpConnectionEStats</a> function to retrieve extended statistics on the TCP connection.

The <a href="https://msdn.microsoft.com/71b9d795-6050-4a1a-9949-2c970801f52c">GetPerTcpConnectionEStats</a> function is designed to use TCP to diagnose performance
   problems in both the network and the application.  If a network based
   application is performing poorly, TCP can determine if the bottleneck
   is in the sender, the receiver or the network itself.  If the
   bottleneck is in the network, TCP can provide specific information
   about its nature.


For information on extended TCP statistics on an IPv6 connection, see the <a href="https://msdn.microsoft.com/291aabe7-a4e7-4cc7-9cf3-4a4bc021e15e">GetPerTcp6ConnectionEStats</a> and <a href="https://msdn.microsoft.com/89ace750-ec32-46cb-8526-233f847ba9f4">SetPerTcp6ConnectionEStats</a> functions.

The <b>SetPerTcpConnectionEStats</b> function can only be called by a user logged on as a member of the Administrators group. If <b>SetPerTcpConnectionEStats</b> is called by a user that is not a member of the Administrators group, the function call will fail and <b>ERROR_ACCESS_DENIED</b> is returned. This function can also fail because of user account control (UAC) on Windows Vista and Windows Server 2008. If an application that contains this function is executed by a user logged on as a member of the Administrators group other than the built-in Administrator, this call will fail unless the application has been marked in the manifest file with a <b>requestedExecutionLevel</b> set to requireAdministrator. If the application on Windows Vista or Windows Server 2008 lacks this manifest file, a user logged on as a member of the Administrators group other than the built-in Administrator must then be executing the application in an enhanced shell as the built-in Administrator (RunAs administrator) for this function to succeed.






## -see-also




<a href="https://msdn.microsoft.com/291aabe7-a4e7-4cc7-9cf3-4a4bc021e15e">GetPerTcp6ConnectionEStats</a>



<a href="https://msdn.microsoft.com/71b9d795-6050-4a1a-9949-2c970801f52c">GetPerTcpConnectionEStats</a>



<a href="https://msdn.microsoft.com/e90c5aa0-3126-489b-af44-bf86cb45a6d1">GetTcpTable</a>



<a href="https://msdn.microsoft.com/36364854-caa8-4652-be8e-f741b36d9fd7">MIB_TCPROW</a>



<a href="https://msdn.microsoft.com/89ace750-ec32-46cb-8526-233f847ba9f4">SetPerTcp6ConnectionEStats</a>



<a href="https://msdn.microsoft.com/68f8f797-06fb-4286-88bc-220c54977575">TCP_BOOLEAN_OPTIONAL</a>



<a href="https://msdn.microsoft.com/a9bf5ad3-a8db-4194-8e47-5a7409391f4c">TCP_ESTATS_BANDWIDTH_RW_v0</a>



<a href="https://msdn.microsoft.com/823cea66-f719-40f6-82bd-572623188446">TCP_ESTATS_DATA_RW_v0</a>



<a href="https://msdn.microsoft.com/35834c9a-2896-4c11-aef7-c55af7f6fef3">TCP_ESTATS_FINE_RTT_RW_v0</a>



<a href="https://msdn.microsoft.com/91c2d5d9-3198-42a7-abf7-077281b491f2">TCP_ESTATS_OBS_REC_RW_v0</a>



<a href="https://msdn.microsoft.com/460ad710-06aa-490a-9bac-5a8c731687e9">TCP_ESTATS_PATH_RW_v0</a>



<a href="https://msdn.microsoft.com/e780ae7b-30c6-4890-8a8b-9e0b2739c176">TCP_ESTATS_REC_RW_v0</a>



<a href="https://msdn.microsoft.com/1bc88d95-24d2-4ca3-9f4a-298d5c08f4de">TCP_ESTATS_SEND_BUFF_RW_v0</a>



<a href="https://msdn.microsoft.com/7fc7fb6a-4486-450f-b60e-8cf07b33c79a">TCP_ESTATS_SND_CONG_RW_v0</a>



<a href="https://msdn.microsoft.com/96f55528-e74a-4360-a7a2-54ba19c3a284">TCP_ESTATS_TYPE</a>
 

 

