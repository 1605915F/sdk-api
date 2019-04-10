---
UID: NF:ntsecapi.LsaLookupNames
title: LsaLookupNames function (ntsecapi.h)
author: windows-sdk-content
description: Retrieves the security identifiers (SIDs) that correspond to an array of user, group, or local group names.
old-location: security\lsalookupnames.htm
tech.root: SecMgmt
ms.assetid: 867604aa-7a39-4da7-b189-a9183461e9a0
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: LsaLookupNames, LsaLookupNames function [Security], _lsa_lsalookupnames, ntsecapi/LsaLookupNames, security.lsalookupnames
ms.topic: function
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
 - AdvApi32Legacy.dll
 - Ext-MS-Win-AdvAPI32-Lsa-L1-1-1.dll
api_name:
 - LsaLookupNames
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# LsaLookupNames function


## -description


The <b>LsaLookupNames</b> function retrieves the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifiers</a> (SIDs) that correspond to an array of user, group, or local group names.

The <b>LsaLookupNames</b> function is superseded by the <a href="https://msdn.microsoft.com/fe219070-6a00-4b8c-b2e4-2ad290a1cb9c">LsaLookupNames2</a> function. Applications should use the <b>LsaLookupNames2</b> function to ensure future compatibility.

The <b>LsaLookupNames</b> function can also retrieve computer accounts. 


## -parameters




### -param PolicyHandle [in]

A handle to a <a href="https://msdn.microsoft.com/4253c7fb-85f5-441d-90bf-492e802ad0f8">Policy</a> object. The handle must have the POLICY_LOOKUP_NAMES access right. For more information, see 
<a href="https://msdn.microsoft.com/66fdc878-d9c4-421c-b79f-9df08984611c">Opening a Policy Object Handle</a>.


### -param Count [in]

Specifies the number of names in the <i>Names</i> array. This is also the number of entries returned in the <i>Sids</i> array.


### -param Names [in]

Pointer to an array of 
<a href="https://msdn.microsoft.com/9e1cf20f-01f9-4813-bf95-e47c5d57dcdc">LSA_UNICODE_STRING</a> structures that contain the names to look up. The strings in these structures can be the names of user, group, or local group accounts, or the names of domains. Domain names can be DNS domain names or NetBIOS domain names. 




For more information about the format of the name strings, see Remarks.


### -param ReferencedDomains [out]

Receives a pointer to an 
<a href="https://msdn.microsoft.com/ddf0afcb-7ec4-42ed-bf40-38ef33f33a0c">LSA_REFERENCED_DOMAIN_LIST</a> structure. The <b>Domains</b> member of this structure is an array that contains an entry for each domain in which a name was found. The <b>DomainIndex</b> member of each entry in the <i>Sids</i> array is the index of the <b>Domains</b> array entry for the domain in which the name was found. 




When you have finished using the returned pointer, free the memory by calling the  
<a href="https://msdn.microsoft.com/6eb3d18f-c54c-4e51-8a4b-b7a3f930cfa9">LsaFreeMemory</a> function. This memory must be freed even when the function fails with the either of the error codes <b>STATUS_NONE_MAPPED</b> or <b>STATUS_SOME_NOT_MAPPED</b>


### -param Sids [out]

Receives a pointer to an array of 
<a href="https://msdn.microsoft.com/1fa8fb74-3e61-4982-aa6b-a0ffe979abd4">LSA_TRANSLATED_SID</a> structures. Each entry in the <i>Sids</i> array contains the SID information for the corresponding entry in the <i>Names</i> array.  




When you have finished using the returned pointer, free the memory by calling the  
<a href="https://msdn.microsoft.com/6eb3d18f-c54c-4e51-8a4b-b7a3f930cfa9">LsaFreeMemory</a> function. This memory must be freed even when the function fails with the either of the error codes <b>STATUS_NONE_MAPPED</b> or <b>STATUS_SOME_NOT_MAPPED</b>


## -returns



If the function succeeds, the function returns  one of the following <b>NTSTATUS</b> values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_SOME_NOT_MAPPED</b></dt>
</dl>
</td>
<td width="60%">
Some of the names could not be translated. This is an informational-level return value.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
All of the names were found and successfully translated.

</td>
</tr>
</table>
 

If the function fails, the return value is the following <b>NTSTATUS</b> value or one of the 
<a href="https://msdn.microsoft.com/en-us/library/ms721859(v=VS.85).aspx">LSA Policy Function Return Values</a>.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_NONE_MAPPED</b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
None of the names were translated.

</td>
</tr>
</table>
 

Use the 
<a href="https://msdn.microsoft.com/fa91794c-c502-4b36-84cc-a8d77c8e9d9f">LsaNtStatusToWinError</a> function to convert the <b>NTSTATUS</b> code to a Windows error code.




## -remarks



Use fully qualified account names (for example, domain_name\user_name) instead of isolated names (for example, user_name). Fully qualified names are unambiguous and provide better performance when the lookup is performed. This function also supports fully qualified DNS names (for example, example.example.com\user_name) and <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">user principal names</a> (UPN) (for example, someone@example.com).

Translation of isolated names introduces the possibility of name collisions because the same name may be used in multiple domains. The 
<b>LsaLookupNames</b> function uses the following algorithm to translate isolated names

<p class="proch"><img alt="" src="../common/wedge.gif"/><b>To translate isolated names</b>

<ol>
<li>If the name is a well-known name, such as Local or Interactive, the function returns the corresponding well-known <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifier</a> (SID).</li>
<li>If the name is the name of the built-in domain, the function returns the SID of that domain.</li>
<li>If the name is the name of the account domain, the function returns the SID of that domain.</li>
<li>If the name is the name of the primary domain, the function returns the SID of that domain.</li>
<li>If the name is one of the names of the trusted domain, the function returns the SID of that domain.</li>
<li>If the name is a user, group, or local group account in the built-in domain, the function returns the SID of that account.</li>
<li>If the name is a user, group, or local group account in the account domain on the local system, the function returns the SID of that account.</li>
<li>If the name is a user, group, or a local group in the primary domain, the function returns the SID of that account.</li>
<li>After looking in the primary domain, the primary domain looks in each of its trusted domains.</li>
<li>Otherwise, the name is not translated.</li>
</ol>
In addition to looking up local accounts, local domain accounts, and explicitly trusted domain accounts, <b>LsaLookupNames</b> can look up the name of any account in any domain in the Windows forest.


#### Examples

For an example that calls this function, see 
<a href="https://msdn.microsoft.com/8845b709-a8f9-4d0f-a4a6-86d23d6b01d5">Translating Between Names and SIDs</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/ddf0afcb-7ec4-42ed-bf40-38ef33f33a0c">LSA_REFERENCED_DOMAIN_LIST</a>



<a href="https://msdn.microsoft.com/1fa8fb74-3e61-4982-aa6b-a0ffe979abd4">LSA_TRANSLATED_SID</a>



<a href="https://msdn.microsoft.com/9e1cf20f-01f9-4813-bf95-e47c5d57dcdc">LSA_UNICODE_STRING</a>



<a href="https://msdn.microsoft.com/6eb3d18f-c54c-4e51-8a4b-b7a3f930cfa9">LsaFreeMemory</a>



<a href="https://msdn.microsoft.com/69051bad-91e7-469d-9010-48ac3d20f8af">LsaLookupSids</a>
 

 

