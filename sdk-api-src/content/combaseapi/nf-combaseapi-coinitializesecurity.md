---
UID: NF:combaseapi.CoInitializeSecurity
title: CoInitializeSecurity function
author: windows-sdk-content
description: Registers security and sets the default security values for the process.
old-location: com\coinitializesecurity.htm
tech.root: com
ms.assetid: e0933741-6b75-4ce1-aa63-6240e4a7130f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CoInitializeSecurity, CoInitializeSecurity function [COM], _com_CoInitializeSecurity, com.coinitializesecurity, combaseapi/CoInitializeSecurity
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: combaseapi.h
req.include-header: Objbase.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Ole32.lib
req.dll: Ole32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ole32.dll
 - API-MS-Win-Core-Com-l1-1-0.dll
 - ComBase.dll
 - API-MS-Win-Core-Com-l1-1-1.dll
 - API-MS-Win-DownLevel-Ole32-l1-1-0.dll
 - API-MS-Win-DownLevel-Ole32-l1-1-1.dll
api_name:
 - CoInitializeSecurity
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CoInitializeSecurity function


## -description


Registers security and sets the default security values for the process.


## -parameters




### -param pSecDesc [in, optional]

The access permissions that a server will use to receive calls. This parameter is used by COM only when a server calls <b>CoInitializeSecurity</b>. Its value is a pointer to one of three types: an AppID, an <a href="https://msdn.microsoft.com/en-us/library/ms694421(v=VS.85).aspx">IAccessControl</a> object, or a <a href="https://msdn.microsoft.com/en-us/library/Aa379561(v=VS.85).aspx">SECURITY_DESCRIPTOR</a>, in absolute format. See the Remarks section for more information.


### -param cAuthSvc [in]

The count of entries in the <i>asAuthSvc</i> parameter. This parameter is used by COM only when a server calls <b>CoInitializeSecurity</b>. If this parameter is 0, no authentication services will be registered and the server cannot receive secure calls. A value of -1 tells COM to choose which authentication services to register, and if this is the case, the <i>asAuthSvc</i> parameter must be <b>NULL</b>. However, Schannel will never be chosen as an authentication service by the server if this parameter is -1.


### -param asAuthSvc [in, optional]

An array of authentication services that a server is willing to use to receive a call. This parameter is used by COM only when a server calls <b>CoInitializeSecurity</b>. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms686648(v=VS.85).aspx">SOLE_AUTHENTICATION_SERVICE</a>.


### -param pReserved1 [in, optional]

This parameter is reserved and must be <b>NULL</b>.


### -param dwAuthnLevel [in]

The default authentication level for the process. Both servers and clients use this parameter when they call <b>CoInitializeSecurity</b>. COM will fail calls that arrive with a lower authentication level. By default, all proxies will use at least this authentication level. This value should contain one of the <a href="https://msdn.microsoft.com/en-us/library/ms678435(v=VS.85).aspx">authentication level constants</a>. By default, all calls to <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> are made at this level.


### -param dwImpLevel [in]

The default impersonation level for proxies. The value of this parameter is used only when the process is a client. It should be a value from the <a href="https://msdn.microsoft.com/en-us/library/ms693790(v=VS.85).aspx">impersonation level constants</a>, except for RPC_C_IMP_LEVEL_DEFAULT, which is not for use with <b>CoInitializeSecurity</b>.

Outgoing calls from the client always use the impersonation level as specified. (It is not negotiated.) Incoming calls to the client can be at any impersonation level. By default, all <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> calls are made with this impersonation level, so even security-aware applications should set this level carefully. To determine which impersonation levels each authentication service supports, see the description of the authentication services in <a href="https://msdn.microsoft.com/en-us/library/ms690278(v=VS.85).aspx">COM and Security Packages</a>. For more information about impersonation levels, see <a href="https://msdn.microsoft.com/b33ca3b0-0423-4338-b3d6-4bb3db3d3e1b">Impersonation</a>. 


### -param pAuthList [in, optional]

A pointer to <a href="https://msdn.microsoft.com/en-us/library/ms680039(v=VS.85).aspx">SOLE_AUTHENTICATION_LIST</a>, which is an array of <a href="https://msdn.microsoft.com/en-us/library/ms680049(v=VS.85).aspx">SOLE_AUTHENTICATION_INFO</a> structures. This list indicates the information for each authentication service that a client can use to call a server. This parameter is used by COM only when a client calls <b>CoInitializeSecurity</b>.


### -param dwCapabilities [in]

Additional capabilities of the client or server, specified by setting one or more <a href="https://msdn.microsoft.com/en-us/library/ms693368(v=VS.85).aspx">EOLE_AUTHENTICATION_CAPABILITIES</a> values. Some of these value cannot be used simultaneously, and some cannot be set when particular authentication services are being used. For more information about these flags, see the Remarks section.


### -param pReserved3 [in, optional]

This parameter is reserved and must be <b>NULL</b>.


## -returns



This function can return the standard return value E_INVALIDARG, as well as the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Indicates success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_E_TOO_LATE</b></dt>
</dl>
</td>
<td width="60%">

<a href="https://msdn.microsoft.com/en-us/library/ms693736(v=VS.85).aspx">CoInitializeSecurity</a> has already been called.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_E_NO_GOOD_SECURITY_PACKAGES</b></dt>
</dl>
</td>
<td width="60%">
The <i>asAuthSvc</i> parameter was not <b>NULL</b>, and none of the authentication services in the list could be registered. Check the results saved in <i>asAuthSvc</i> for authentication service–specific error codes.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUT_OF_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Out of memory.

</td>
</tr>
</table>
 




## -remarks



The <b>CoInitializeSecurity</b> function initializes the security layer and sets the specified values as the security default. If a process does not call <b>CoInitializeSecurity</b>, COM calls it automatically the first time an interface is marshaled or unmarshaled, registering the system default security. No default security packages are registered until then.



This function is called exactly once per process, either explicitly or implicitly. It can be called by the client, server, or both. For legacy applications and other applications that do not explicitly call <b>CoInitializeSecurity</b>, COM calls this function implicitly with values from the registry. If you set processwide security using the registry and then call <b>CoInitializeSecurity</b>, the <a href="https://msdn.microsoft.com/en-us/library/ms682359(v=VS.85).aspx">AppID</a> registry values will be ignored and the <b>CoInitializeSecurity</b> values will be used.

<b>CoInitializeSecurity</b> can be used to override both computer-wide access permissions and application-specific access permissions, but not to override the computer-wide restriction policy.



If <i>pSecDesc</i> points to an AppID, the EOAC_APPID flag must be set in <i>dwCapabilities</i> and, when the EOAC_APPID flag is set, all other parameters to <b>CoInitializeSecurity</b> are ignored. <b>CoInitializeSecurity</b> looks for the authentication level under the <b>AppID</b> key in the registry and uses it to determine the default security. For more information about how the <b>AppID</b> key is used to set security, see <a href="https://msdn.microsoft.com/en-us/library/ms687317(v=VS.85).aspx">Setting Process-Wide Security Through the Registry</a>.



If <i>pSecDesc</i> is a pointer to an <a href="https://msdn.microsoft.com/en-us/library/ms694421(v=VS.85).aspx">IAccessControl</a> object, the EOAC_ACCESS_CONTROL flag must be set and <i>dwAuthnLevel</i> cannot be none. The <b>IAccessControl</b> object is used to determine who can call the process. DCOM will <a href="https://msdn.microsoft.com/en-us/library/ms691379(v=VS.85).aspx">AddRef</a> the <b>IAccessControl</b> and will <a href="https://msdn.microsoft.com/en-us/library/ms682317(v=VS.85).aspx">Release</a> it when <a href="https://msdn.microsoft.com/en-us/library/ms688715(v=VS.85).aspx">CoUninitialize</a> is called. The state of the <b>IAccessControl</b> object should not be changed.



If <i>pSecDesc</i> is a pointer to a <a href="https://msdn.microsoft.com/en-us/library/Aa379561(v=VS.85).aspx">SECURITY_DESCRIPTOR</a>, neither the EOAC_APPID nor the EOAC_ACCESS_CONTROL flag can be set in <i>dwCapabilities</i>. The owner and group of the <b>SECURITY_DESCRIPTOR</b> must be set, and until DCOM supports auditing, the system ACL must be <b>NULL</b>. The access-control entries (ACEs) in the discretionary ACL (DACL) of the <b>SECURITY_DESCRIPTOR</b> are used to find out which callers are permitted to connect to the process's objects. A DACL with no ACEs allows no access, while a <b>NULL</b> DACL will allow calls from anyone. For more information on ACLs and ACEs, see <a href="https://msdn.microsoft.com/en-us/library/Aa374876(v=VS.85).aspx">Access Control Model</a>. Applications should call <a href="https://msdn.microsoft.com/d9fd2e44-5782-40c9-a1cf-1788ca7afc50">AccessCheck</a> (not <a href="https://msdn.microsoft.com/24a98229-11e4-45ef-988b-c2cf831275e7">IsValidSecurityDescriptor</a>) to ensure that their <b>SECURITY_DESCRIPTOR</b> is correctly formed prior to calling <b>CoInitializeSecurity</b>.



Passing <i>pSecDesc</i> as <b>NULL</b> is strongly discouraged. An appropriate alternative might be to use a <a href="https://msdn.microsoft.com/en-us/library/Aa379561(v=VS.85).aspx">SECURITY_DESCRIPTOR</a> that allows Everyone. If <i>pSecDesc</i> is <b>NULL</b>, the flags in <i>dwCapabilities</i> determine how <b>CoInitializeSecurity</b> defines the access permissions that a server will use, as follows: 



<ul>
<li>If the EOAC_APPID flag is set, <b>CoInitializeSecurity</b> will look up the application's .exe name in the registry and use the AppID stored there.</li>
<li>If the EOAC_ACCESS_CONTROL flag is set, <b>CoInitializeSecurity</b> will return an error.
</li>
<li>If neither the EOAC_APPID flag nor the EOAC_ACCESS_CONTROL flag is set, <b>CoInitializeSecurity</b> allows all callers including Local and Remote Anonymous Users.
</li>
</ul>
The <b>CoInitializeSecurity</b> function returns an error if both the EOAC_APPID and EOAC_ACCESS_CONTROL flags are set in <i>dwCapabilities</i>.





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms692692(v=VS.85).aspx">CoSetProxyBlanket</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693319(v=VS.85).aspx">Security in COM</a>
 

 

