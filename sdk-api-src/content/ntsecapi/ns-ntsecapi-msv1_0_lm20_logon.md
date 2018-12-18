---
UID: NS:ntsecapi._MSV1_0_LM20_LOGON
title: MSV1_0_LM20_LOGON
author: windows-sdk-content
description: Contains logon information used in network logons.
old-location: security\msv1_0_lm20_logon.htm
tech.root: secauthn
ms.assetid: 0736ab5b-a475-4593-a15e-970b5d4c64d0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMSV1_0_LM20_LOGON, MSV1_0_ALLOW_MSVCHAPV2, MSV1_0_ALLOW_SERVER_TRUST_ACCOUNT, MSV1_0_ALLOW_WORKSTATION_TRUST_ACCOUNT, MSV1_0_CHECK_LOGONHOURS_FOR_S4U, MSV1_0_CLEARTEXT_PASSWORD_ALLOWED, MSV1_0_CLEARTEXT_PASSWORD_SUPPLIED, MSV1_0_DONT_TRY_GUEST_ACCOUNT, MSV1_0_INTERNET_DOMAIN, MSV1_0_LM20_LOGON, MSV1_0_LM20_LOGON structure [Security], MSV1_0_RETURN_PASSWORD_EXPIRY, MSV1_0_RETURN_PROFILE_PATH, MSV1_0_RETURN_USER_PARAMETERS, MSV1_0_S4U2SELF, MSV1_0_TRY_GUEST_ACCOUNT_ONLY, MSV1_0_TRY_SPECIFIED_DOMAIN_ONLY, MSV1_0_UPDATE_LOGON_STATISTICS, MSV1_0_USE_CLIENT_CHALLENGE, MSV1_0_USE_DOMAIN_FOR_ROUTING_ONLY, PMSV1_0_LM20_LOGON, PMSV1_0_LM20_LOGON structure pointer [Security], _lsa_msv1_0_lm20_logon, ntsecapi/MSV1_0_LM20_LOGON, ntsecapi/PMSV1_0_LM20_LOGON, security.msv1_0_lm20_logon"
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Ntsecapi.h
api_name:
 - MSV1_0_LM20_LOGON
product: Windows
targetos: Windows
req.typenames: MSV1_0_LM20_LOGON, *PMSV1_0_LM20_LOGON
req.redist: 
---

# MSV1_0_LM20_LOGON structure


## -description


The <b>MSV1_0_LM20_LOGON</b> structure contains logon information used in network logons.

It is used by 
<a href="https://msdn.microsoft.com/75968d53-5af2-4d77-9486-26403b73c954">LsaLogonUser</a>.


## -struct-fields




### -field MessageType

A <a href="https://msdn.microsoft.com/03bf43f0-44f4-40c6-8d5d-381f36ebdd0e">MSV1_0_LOGON_SUBMIT_TYPE</a> value that specifies the type of logon being requested. This member must be set to <b>MsV1_0Lm20Logon</b> or <b>MsV1_0NetworkLogon</b>. 




If this member is set to <b>MsV1_0Lm20Logon</b>, the MSV1_0 package ignores the <b>ParameterControl</b> member.


### -field LogonDomainName

A <a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> that contains the name of the logon domain. The specified domain name must be a Windows domain (or mixed domain) that is in the trusted domain list of this computer. If the logon domain name is not known (for example, for clients that do not supply this information), this member should be passed in as a zero-length string. This domain is the authenticating authority.


### -field UserName

A <a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> that represents the account name of the user. The name can be up to 255 bytes long. The name is treated as case insensitive.


### -field Workstation

A <a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> that contains the computer name of the client workstation from which the user logon request was initiated.


### -field ChallengeToClient

Contains the challenge returned from a previous call to 
<a href="https://msdn.microsoft.com/b891fa60-28b3-4819-9a92-e4524677fa4f">LsaCallAuthenticationPackage</a>, when <b>MsV1_0Lm20ChallengeRequest</b> was specified as the message type. For more information, see the description of <b>MsV1_0Lm20ChallengeRequest</b> in 
<a href="https://msdn.microsoft.com/9498558c-8daf-4dfb-aa1c-0598154ca8c4">MSV1_0_PROTOCOL_MESSAGE_TYPE</a>. This enables the <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">authentication package</a> to determine whether the challenge response is correct.


### -field CaseSensitiveChallengeResponse

Contains some function of the case-sensitive <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">Unicode</a> password of the client. Typically, it will be the <b>ChallengeToClient</b> member encrypted by a case-sensitive version of the password. 




Some clients will simply supply the <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">plaintext</a> case-sensitive <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">Unicode</a> password. In that case, this member points to that <i>plaintext</i> password. The 
<a href="https://msdn.microsoft.com/8b85588d-0a79-43af-b526-7a5fc8248f99">MSV1_0 Authentication Package</a> may accept this nonencrypted form depending on a configuration option.

Some clients do not support case-sensitive <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">Unicode</a> passwords. In that case, this member should  contain a zero-length string.


### -field CaseInsensitiveChallengeResponse

Contains some function of the case-insensitive multiple-byte character set (MBCS) password of the client. Typically, it will be the <b>ChallengeToClient</b> member encrypted by a case-insensitive version of the password. 




Clients that  support only MBCS and not <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">Unicode</a>  supply a <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">plaintext</a> case-insensitive MBCS password. In that case, this member points to that <i>plaintext</i> password. The MSV1_0 authentication package will accept this nonencrypted form depending on a configuration option.


### -field ParameterControl

Specifies attributes of the other parameters. This can be one or more of the following flags.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_CLEARTEXT_PASSWORD_ALLOWED"></a><a id="msv1_0_cleartext_password_allowed"></a><dl>
<dt><b>MSV1_0_CLEARTEXT_PASSWORD_ALLOWED</b></dt>
<dt>02</dt>
</dl>
</td>
<td width="60%">
LanMan2.0 or LanMan1.0 send a <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">plaintext</a> password instead of a challenge response. To allow plaintext passwords to be used in the NetworkLogon message, an application must supply this flag.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_UPDATE_LOGON_STATISTICS"></a><a id="msv1_0_update_logon_statistics"></a><dl>
<dt><b>MSV1_0_UPDATE_LOGON_STATISTICS</b></dt>
<dt>04</dt>
</dl>
</td>
<td width="60%">
Update the logon statistics for the account. If this flag is not set, the bad password count is set to zero upon successful logon.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_RETURN_USER_PARAMETERS"></a><a id="msv1_0_return_user_parameters"></a><dl>
<dt><b>MSV1_0_RETURN_USER_PARAMETERS</b></dt>
<dt>08</dt>
</dl>
</td>
<td width="60%">
If this flag is specified, the <b>UserParameters</b> member of the 
<a href="https://msdn.microsoft.com/4bf69171-1f92-40df-ab0f-cd6790ce34f1">MSV1_0_LM20_LOGON_PROFILE</a> return buffer is valid.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_DONT_TRY_GUEST_ACCOUNT"></a><a id="msv1_0_dont_try_guest_account"></a><dl>
<dt><b>MSV1_0_DONT_TRY_GUEST_ACCOUNT</b></dt>
<dt>10</dt>
</dl>
</td>
<td width="60%">
Prevents the user from logging on with a guest account.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_ALLOW_SERVER_TRUST_ACCOUNT"></a><a id="msv1_0_allow_server_trust_account"></a><dl>
<dt><b>MSV1_0_ALLOW_SERVER_TRUST_ACCOUNT</b></dt>
<dt>20</dt>
</dl>
</td>
<td width="60%">
If this flag is set, domain controller accounts can be used for authentication; otherwise, only user accounts can be used.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_RETURN_PASSWORD_EXPIRY"></a><a id="msv1_0_return_password_expiry"></a><dl>
<dt><b>MSV1_0_RETURN_PASSWORD_EXPIRY</b></dt>
<dt>40</dt>
</dl>
</td>
<td width="60%">
Causes the password expiration time to be returned in the <b>LogoffTime</b> member of the <a href="https://msdn.microsoft.com/4bf69171-1f92-40df-ab0f-cd6790ce34f1">MSV1_0_LM20_LOGON_PROFILE</a> structure returned in the output buffer.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_USE_CLIENT_CHALLENGE"></a><a id="msv1_0_use_client_challenge"></a><dl>
<dt><b>MSV1_0_USE_CLIENT_CHALLENGE</b></dt>
<dt>80</dt>
</dl>
</td>
<td width="60%">
 Denotes that the CaseInsensitiveChallengeResponse contains a client challenge in the first 8 bytes.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_TRY_GUEST_ACCOUNT_ONLY"></a><a id="msv1_0_try_guest_account_only"></a><dl>
<dt><b>MSV1_0_TRY_GUEST_ACCOUNT_ONLY</b></dt>
<dt>100</dt>
</dl>
</td>
<td width="60%">
Causes the user to log on using the guest account.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_RETURN_PROFILE_PATH"></a><a id="msv1_0_return_profile_path"></a><dl>
<dt><b>MSV1_0_RETURN_PROFILE_PATH</b></dt>
<dt>200</dt>
</dl>
</td>
<td width="60%">
Returns the profile path for <a href="https://msdn.microsoft.com/f1caccd2-3453-448e-b194-bf899eff8091">Encrypting File System</a> (EFS). The profile path is used by EFS to locate the profile of the user and find the user's keys for encrypting and decrypting files. This information is not returned to the caller; it is stored within the LSA and used by internal processes.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_TRY_SPECIFIED_DOMAIN_ONLY"></a><a id="msv1_0_try_specified_domain_only"></a><dl>
<dt><b>MSV1_0_TRY_SPECIFIED_DOMAIN_ONLY</b></dt>
<dt>400</dt>
</dl>
</td>
<td width="60%">
In normal operation, the <b>LogonDomainName</b> member is used as a suggestion. The package (using the NetLogon service) will continue passing the logon request to domain controllers higher in the trusted domain path until one authoritatively rejects the logon.
								

This flag overrides that behavior so that only the specified domain controller will attempt to process the logon. If <b>LogonDomainName</b> is blank, the logon will not be attempted.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_ALLOW_WORKSTATION_TRUST_ACCOUNT"></a><a id="msv1_0_allow_workstation_trust_account"></a><dl>
<dt><b>MSV1_0_ALLOW_WORKSTATION_TRUST_ACCOUNT</b></dt>
<dt>800</dt>
</dl>
</td>
<td width="60%">
 Permits remote-boot clients to log on using a computer account.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_CLEARTEXT_PASSWORD_SUPPLIED"></a><a id="msv1_0_cleartext_password_supplied"></a><dl>
<dt><b>MSV1_0_CLEARTEXT_PASSWORD_SUPPLIED</b></dt>
<dt>4000</dt>
</dl>
</td>
<td width="60%">
 Permits the user of a clear text password.

<b>Windows XP and Windows Server 2003:  </b>Not supported.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_USE_DOMAIN_FOR_ROUTING_ONLY"></a><a id="msv1_0_use_domain_for_routing_only"></a><dl>
<dt><b>MSV1_0_USE_DOMAIN_FOR_ROUTING_ONLY</b></dt>
<dt>8000</dt>
</dl>
</td>
<td width="60%">
 Permits the domain to be used for routing only. 

<b>Windows XP and Windows Server 2003:  </b>Not supported.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_ALLOW_MSVCHAPV2"></a><a id="msv1_0_allow_msvchapv2"></a><dl>
<dt><b>MSV1_0_ALLOW_MSVCHAPV2</b></dt>
<dt>10000</dt>
</dl>
</td>
<td width="60%">
 Permits SubAuthentication log on.

<b>Windows XP and Windows Server 2003:  </b>Not supported.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_S4U2SELF"></a><a id="msv1_0_s4u2self"></a><dl>
<dt><b>MSV1_0_S4U2SELF</b></dt>
<dt>20000</dt>
</dl>
</td>
<td width="60%">
 Permits S4U clients to log on without a password.

<b>Windows Vista, Windows Server 2003 with SP2, Windows XP and Windows Server 2003:  </b>Not supported.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_CHECK_LOGONHOURS_FOR_S4U"></a><a id="msv1_0_check_logonhours_for_s4u"></a><dl>
<dt><b>MSV1_0_CHECK_LOGONHOURS_FOR_S4U</b></dt>
<dt>40000</dt>
</dl>
</td>
<td width="60%">
 Check the log on hours for a S4U log on client.

<b>Windows Vista, Windows Server 2003 with SP2, Windows XP and Windows Server 2003:  </b>Not supported.

</td>
</tr>
<tr>
<td width="40%"><a id="MSV1_0_INTERNET_DOMAIN"></a><a id="msv1_0_internet_domain"></a><dl>
<dt><b>MSV1_0_INTERNET_DOMAIN</b></dt>
<dt>80000</dt>
</dl>
</td>
<td width="60%">
 Permits log on for Internet users. This flag should be used by calls from authentication packages directly and not from netlogon.

<b>Windows 7, Windows Server 2008 R2, Windows Vista, Windows Server 2008, Windows XP and Windows Server 2003:  </b>Not supported.

</td>
</tr>
</table>
 


## -remarks



If the <b>UserName</b>, <b>CaseSensitiveChallengeResponse</b>, and <b>CaseInsensitiveChallengeResponse</b> members all contain zero-length strings, an anonymous token will be generated for the logon. This anonymous token gives the user no ability to access protected system resources but does allow access to nonprotected system resources. The server uses this method to support a <b>NULL</b> session.




## -see-also




<a href="https://msdn.microsoft.com/b891fa60-28b3-4819-9a92-e4524677fa4f">LsaCallAuthenticationPackage</a>



<a href="https://msdn.microsoft.com/75968d53-5af2-4d77-9486-26403b73c954">LsaLogonUser</a>



<a href="https://msdn.microsoft.com/4bf69171-1f92-40df-ab0f-cd6790ce34f1">MSV1_0_LM20_LOGON_PROFILE</a>



<a href="https://msdn.microsoft.com/03bf43f0-44f4-40c6-8d5d-381f36ebdd0e">MSV1_0_LOGON_SUBMIT_TYPE</a>



<a href="https://msdn.microsoft.com/9498558c-8daf-4dfb-aa1c-0598154ca8c4">MSV1_0_PROTOCOL_MESSAGE_TYPE</a>
 

 

