---
UID: NF:netioapi.DeleteUnicastIpAddressEntry
title: DeleteUnicastIpAddressEntry function (netioapi.h)
author: windows-sdk-content
description: Deletes an existing unicast IP address entry on the local computer.
old-location: iphlp\deleteunicastipaddressentry.htm
tech.root: IpHlp
ms.assetid: a630397a-ef4a-40c2-b2e7-3e85cd9e8029
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DeleteUnicastIpAddressEntry, DeleteUnicastIpAddressEntry function [IP Helper], iphlp.deleteunicastipaddressentry, netioapi/DeleteUnicastIpAddressEntry
ms.topic: function
req.header: netioapi.h
req.include-header: Iphlpapi.h
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
 - DeleteUnicastIpAddressEntry
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DeleteUnicastIpAddressEntry function


## -description


The 
<b>DeleteUnicastIpAddressEntry</b> function   deletes an existing unicast IP address entry on the local computer. 


## -parameters




### -param Row [in]

A pointer to a 
<a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a> structure entry for an existing unicast IP address entry to delete from the local computer.


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
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
An invalid parameter was passed to the function. This error is returned if a <b>NULL</b> pointer is passed in the <i>Row</i> parameter, the <b>Address</b> member of the <a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a> pointed to by the <i>Row</i> parameter was not set to a valid unicast IPv4 or IPv6 address, or both the <b>InterfaceLuid</b> or <b>InterfaceIndex</b> members of the <b>MIB_UNICASTIPADDRESS_ROW</b> pointed to by the <i>Row</i> parameter were unspecified.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The specified interface could not be found. This error is returned if the  network interface specified by the <b>InterfaceLuid</b> or <b>InterfaceIndex</b> member of the <a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a> pointed to by the <i>Row</i> parameter could not be found.  

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The request is not supported. This error is returned if no IPv4 stack is on the local computer and an IPv4 address was specified in the <b>Address</b> member <a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a> pointed to by the <i>Row</i> parameter. This error is also returned if no IPv6 stack is on the local computer and an IPv6 address was specified in the <b>Address</b> member.

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



The <b>DeleteUnicastIpAddressEntry</b> function is defined on Windows Vista and later. 

The <b>DeleteUnicastIpAddressEntry</b> function is used to delete an existing <a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a> structure entry on the local computer.  

On input, the <b>Address</b> member in the <a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a> structure pointed to by the <i>Row</i> parameter must be set to a valid unicast IPv4 or IPv6 address and family. In addition, at least one of the following members in the <b>MIB_UNICASTIPADDRESS_ROW</b> structure pointed to the <i>Row</i> parameter must be initialized:
    the <b>InterfaceLuid</b> or <b>InterfaceIndex</b>.

    The fields are used in the order listed above. So if the <b>InterfaceLuid</b> is specified, then this member is used to determine the interface. If no value was set for the  <b>InterfaceLuid</b> member (the values of this member was set to zero), then the <b>InterfaceIndex</b> member is next used to determine the interface. 

If the function is successful, the existing IP address represented by the <i>Row</i> parameter was deleted. 

The <a href="https://msdn.microsoft.com/bdafc4a4-5f3c-4dd5-ba9b-4f6045a82652">GetUnicastIpAddressTable</a> function can be called to enumerate the unicast IP address entries on a local computer. The <a href="https://msdn.microsoft.com/d5475c09-05dd-41d7-80ff-63c52d78468c">GetUnicastIpAddressEntry</a> function can be called to retrieve a specific existing unicast IP address entry.

The <b>DeleteUnicastIpAddressEntry</b> function can only be called by a user logged on as a member of the Administrators group. If <b>DeleteUnicastIpAddressEntry</b> is called by a user that is not a member of the Administrators group, the function call will fail and <b>ERROR_ACCESS_DENIED</b> is returned. This function can also fail because of user account control (UAC) on Windows Vista and later. If an application that contains this function is executed by a user logged on as a member of the Administrators group other than the built-in Administrator, this call will fail unless the application has been marked in the manifest file with a <b>requestedExecutionLevel</b> set to requireAdministrator. If the application lacks this manifest file, a user logged on as a member of the Administrators group other than the built-in Administrator must then be executing the application in an enhanced shell as the built-in Administrator (RunAs administrator) for this function to succeed.






## -see-also




<a href="https://msdn.microsoft.com/8afca4e9-a4c4-4f93-bb4d-25e2eea71ae0">CreateUnicastIpAddressEntry</a>



<a href="https://msdn.microsoft.com/d5475c09-05dd-41d7-80ff-63c52d78468c">GetUnicastIpAddressEntry</a>



<a href="https://msdn.microsoft.com/bdafc4a4-5f3c-4dd5-ba9b-4f6045a82652">GetUnicastIpAddressTable</a>



<a href="https://msdn.microsoft.com/2de88e92-5fa5-4d8d-9448-67a33bf02f05">IP Helper Function Reference</a>



<a href="https://msdn.microsoft.com/8cbdd972-060a-4e18-9490-450df21936ea">InitializeUnicastIpAddressEntry</a>



<a href="https://msdn.microsoft.com/f329bafd-9e83-4754-a9a9-e7e111229c90">MIB_UNICASTIPADDRESS_ROW</a>



<a href="https://msdn.microsoft.com/b064494c-d0d5-4570-b255-4cc95412fd3a">MIB_UNICASTIPADDRESS_TABLE</a>



<a href="https://msdn.microsoft.com/56945aa2-ca1e-44b3-9765-d862978a9dbe">NotifyUnicastIpAddressChange</a>



<a href="https://msdn.microsoft.com/906a3895-2e42-4bed-90a3-7c10487d76cb">SetUnicastIpAddressEntry</a>
 

 

