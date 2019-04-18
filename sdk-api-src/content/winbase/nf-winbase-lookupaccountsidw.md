---
UID: NF:winbase.LookupAccountSidW
title: LookupAccountSidW function (winbase.h)
author: windows-sdk-content
description: Accepts a security identifier (SID) as input. It retrieves the name of the account for this SID and the name of the first domain on which this SID is found.
old-location: security\lookupaccountsid.htm
tech.root: SecAuthZ
ms.assetid: b8a44ffc-86e1-4f79-ad51-8340da9eaefd
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: LookupAccountSid, LookupAccountSid function [Security], LookupAccountSidA, LookupAccountSidW, _win32_lookupaccountsid, security.lookupaccountsid, winbase/LookupAccountSid, winbase/LookupAccountSidA, winbase/LookupAccountSidW
ms.topic: function
req.header: winbase.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: LookupAccountSidW (Unicode) and LookupAccountSidA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Advapi32.lib
req.dll: Advapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Advapi32.dll
 - API-MS-Win-DownLevel-AdvAPI32-l4-1-0.dll
 - advapi32legacy.dll
 - API-MS-Win-security-lsalookup-l2-1-0.dll
 - API-MS-Win-security-lsalookup-l2-1-1.dll
 - API-MS-Win-Security-LSALookup-L2-1-2.dll
 - API-MS-Win-Security-LSALookup-Ansi-L2-1-0.dll
api_name:
 - LookupAccountSid
 - LookupAccountSidA
 - LookupAccountSidW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# LookupAccountSidW function


## -description


The <b>LookupAccountSid</b> function accepts a <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifier</a> (SID) as input. It retrieves the name of the account for this SID and the name of the first domain on which this SID is found.


## -parameters




### -param lpSystemName [in, optional]

A pointer to a <b>null</b>-terminated character string that specifies the target computer. This string can be the name of a remote computer. If this parameter is <b>NULL</b>, the account name translation begins on the local system. If the name cannot be resolved on the local system, this function will try to resolve the name using domain controllers trusted by the local system. Generally, specify a value for  <i>lpSystemName</i> only when the  account is in an untrusted domain and the   name of a computer in that domain is known.


### -param Sid [in]

A pointer to the 
<a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">SID</a> to look up.


### -param Name [out, optional]

A pointer to a buffer that receives a <b>null</b>-terminated string that contains the account name that corresponds to the <i>lpSid</i> parameter.


### -param cchName [in, out]

On input, specifies the size, in <b>TCHAR</b>s, of the <i>lpName</i> buffer. If the function fails because the buffer is too small or if <i>cchName</i> is zero, <i>cchName</i> receives the required buffer size, including the terminating <b>null</b> character.


### -param ReferencedDomainName [out, optional]

A pointer to a buffer that receives a <b>null</b>-terminated string that contains the name of the domain where the account name was found.

On a server, the domain name returned for most accounts in the security database of the local computer is the name of the domain for which the server is a domain controller.
						

On a workstation, the domain name returned for most accounts in the security database of the local computer is the name of the computer as of the last start of the system (backslashes are excluded). If the name of the computer changes, the old name continues to be returned as the domain name until the system is restarted.

Some accounts are predefined by the system. The domain name returned for these accounts is BUILTIN.


### -param cchReferencedDomainName [in, out]

On input, specifies the size, in <b>TCHAR</b>s, of the <i>lpReferencedDomainName</i> buffer. If the function fails because the buffer is too small or if <i>cchReferencedDomainName</i> is zero, <i>cchReferencedDomainName</i> receives the required buffer size, including the terminating <b>null</b> character.


### -param peUse [out]

A pointer to a variable that receives a 
<a href="https://msdn.microsoft.com/4e6af6bd-056b-4f5a-b223-57a673c3fcfa">SID_NAME_USE</a> value that indicates the type of the account.


## -returns



If the function succeeds, the function returns nonzero.

If the function fails, it returns zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The <b>LookupAccountSid</b> function attempts to find a name for the specified SID by first checking a list of well-known SIDs. If the supplied SID does not correspond to a well-known SID, the function checks built-in and administratively defined local accounts. Next, the function checks the primary domain. <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">Security identifiers</a> not recognized by the primary domain are checked against the trusted domains that correspond to their SID prefixes.

If the function cannot find an account name for the SID, <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> returns ERROR_NONE_MAPPED. This can occur if a network time-out prevents the function from finding the name. It also occurs for SIDs that have no corresponding account name, such as a <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">logon SID</a> that identifies a <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">logon session</a>.

In addition to looking up SIDs for local accounts, local domain accounts, and explicitly trusted domain accounts, <b>LookupAccountSid</b> can look up SIDs for any account in any domain in the forest, including SIDs that appear only in the SIDhistory field of an account in the forest. The SIDhistory field stores former SIDs of an account that has been moved from another domain. To look up a SID, <b>LookupAccountSid</b> queries the global catalog of the forest. 


#### Examples

For an example that uses this function, see <a href="https://msdn.microsoft.com/f895dfef-75ad-419c-95d0-6480bdf9c769">Searching for a SID in an Access Token</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/d9ce4ec5-5c09-4b33-93a1-39638a925986">Access Control Overview</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa375742(v=VS.85).aspx">Basic Access Control Functions</a>



<a href="https://msdn.microsoft.com/ef41de63-4ab5-40c6-8b16-b960e1308b5b">EqualPrefixSid</a>



<a href="https://msdn.microsoft.com/72855539-469a-4289-99cc-eae2ed89901f">LookupAccountName</a>



<a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">SID</a>



<a href="https://msdn.microsoft.com/4e6af6bd-056b-4f5a-b223-57a673c3fcfa">SID_NAME_USE</a>
 

 

