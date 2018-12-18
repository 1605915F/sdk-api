---
UID: NF:dsparse.DsMakeSpnW
title: DsMakeSpnW function
author: windows-sdk-content
description: Constructs a service principal name (SPN) that identifies a service instance.
old-location: ad\dsmakespn.htm
tech.root: ad
ms.assetid: fca3c59c-bb81-42a0-acd3-2e55c902febe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DsMakeSpn, DsMakeSpn function [Active Directory], DsMakeSpnA, DsMakeSpnW, _glines_dsmakespn, ad.dsmakespn, dsparse/DsMakeSpn, dsparse/DsMakeSpnA, dsparse/DsMakeSpnW
ms.topic: function
req.header: dsparse.h
req.include-header: Ntdsapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: DsMakeSpnW (Unicode) and DsMakeSpnA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Ntdsapi.lib
req.dll: Ntdsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ntdsapi.dll
api_name:
 - DsMakeSpn
 - DsMakeSpnA
 - DsMakeSpnW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DsMakeSpnW function


## -description


The <b>DsMakeSpn</b> function constructs a service principal name (SPN) that identifies a service instance.

A client application uses this function to compose an SPN, which it uses to authenticate the service instance. For example, the client can pass an SPN in the <i>pszTargetName</i> parameter of the 
<a href="https://msdn.microsoft.com/library/Aa375506(v=VS.85).aspx">InitializeSecurityContext</a> function.


## -parameters




### -param ServiceClass [in]

Pointer to a constant null-terminated string that specifies the class of the service. This parameter can be any string unique to that service; either the protocol name, for example, ldap, or the string form of a GUID are acceptable.


### -param ServiceName [in]

Pointer to a constant null-terminated string that specifies the DNS name, NetBIOS name, or distinguished name (DN). This parameter must be non-<b>NULL</b>.

For more information about how the <i>ServiceName</i>, <i>InstanceName</i> and <i>InstancePort</i> parameters are used to compose an SPN, see the following Remarks section.


### -param InstanceName [in, optional]

Pointer to a constant null-terminated string that specifies the DNS name or IP address of the host for an instance of the service.

If <i>ServiceName</i> specifies the DNS or NetBIOS name of the service host computer, the <i>InstanceName</i> parameter must be <b>NULL</b>.

If <i>ServiceName</i> specifies a DNS domain name, the name of a DNS SRV record, or a distinguished name, such as the DN of a service connection point, the <i>InstanceName</i> parameter must specify the DNS or NetBIOS name of the service host computer.


### -param InstancePort [in]

Port number for an instance of the service. Use 0 for the default port. If this parameter is zero, the SPN does not include a port number.


### -param Referrer [in, optional]

Pointer to a constant null-terminated string that specifies the DNS name of the host that gave an IP address referral. This parameter is ignored unless the <i>ServiceName</i> parameter specifies an IP address.


### -param pcSpnLength [in, out]

Pointer to a variable that contains the length, in characters, of the buffer that will receive the new constructed SPN. This value may be 0 to request the final buffer size in advance.

The <i>pcSpnLength</i> parameter also receives the actual length of the SPN created, including the terminating null character.


### -param pszSpn [out]

Pointer to a null-terminated string that receives the constructed SPN. This buffer should be the length specified by <i>pcSpnLength</i>. The <i>pszSpn</i> parameter may be <b>NULL</b> to request the final buffer size in advance.


## -returns



If the function returns an SPN, the return value is <b>ERROR_SUCCESS</b>. If the function fails, the return value can be one of the following error codes.




## -remarks



The format of the SPN produced by the <b>DsMakeSpn</b> function depends on the input parameters. There are two basic formats. Both formats begin with the <i>ServiceClass</i> string followed by a host computer name and an optional <i>InstancePort</i> component.

<div class="alert"><b>Note</b>  This format is used by host-based services.</div>
<div> </div>
<p class="proch"><img alt="" src="../common/wedge.gif"/><b>To produce an SPN with the "&lt;ServiceClass&gt;/&lt;host&gt;" format</b>

<ol>
<li>Set the <i>ServiceName</i> parameter to the DNS name of the host computer for the service instance. This is the host component of the SPN.</li>
<li>Set the <i>InstanceName</i> and <i>Referrer</i> parameters to <b>NULL</b>.</li>
<li>
Set the <i>InstancePort</i> parameter to zero. If <i>InstancePort</i> is nonzero, the SPN has the following format:

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>&lt;service class&gt;/&lt;host&gt;:&lt;instance port&gt;/&lt;referrer&gt;</pre>
</td>
</tr>
</table></span></div>
</li>
</ol>
<div class="alert"><b>Note</b>  This format is used by replicable services.</div>
<div> </div>
<p class="proch"><img alt="" src="../common/wedge.gif"/><b>To produce an SPN with the "&lt;ServiceClass&gt;/&lt;host&gt;:&lt;InstancePort&gt;" format</b>

<ol>
<li>Set the <i>InstanceName</i> parameter to the DNS name of the host computer for the service instance. This is the host component.</li>
<li>Set the <i>ServiceName</i> parameter to a string that identifies an instance of the service. For example, it could be the distinguished name of the service connection point for this service instance.</li>
<li>Set the <i>Referrer</i> parameter to <b>NULL</b>.</li>
<li>
Set the <i>InstancePort</i> parameter to zero. If <i>InstancePort</i> is nonzero, the SPN has the following format:

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>&lt;service class&gt;/&lt;host&gt;:&lt;instance port&gt;/&lt;service name&gt;</pre>
</td>
</tr>
</table></span></div>
</li>
</ol>
The <i>Referrer</i> parameter is used only if the <i>ServiceName</i> parameter specifies the IP address of the service's host computer. In this case, <i>Referrer</i> specifies the DNS name of the computer that gave the IP address as a referral. The SPN has the following format:

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>&lt;service class&gt;/&lt;host&gt;:&lt;instance port&gt;/&lt;referrer&gt;</pre>
</td>
</tr>
</table></span></div>
where the host component is the <i>InstanceName</i> string or the <i>ServiceName</i> string if <i>InstanceName</i> is <b>NULL</b>, and the <i>InstancePort</i> component is optional.

String parameters cannot include the forward slash (/) character, as it is used to separate the components of the SPN.




## -see-also




<a href="https://msdn.microsoft.com/a92783c2-ffb8-473e-8484-1c05ca5453ff">Domain Controller and Replication Management Functions</a>



<a href="https://msdn.microsoft.com/library/Aa375506(v=VS.85).aspx">InitializeSecurityContext</a>
 

 

