---
UID: NS:winnt._PRIVILEGE_SET
title: PRIVILEGE_SET (winnt.h)
author: windows-sdk-content
description: Specifies a set of privileges.
old-location: security\privilege_set.htm
tech.root: SecAuthZ
ms.assetid: 2ee5615c-f684-4062-a6cb-e43e9de3a2fb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PPRIVILEGE_SET, PPRIVILEGE_SET, PPRIVILEGE_SET structure pointer [Security], PRIVILEGE_SET, PRIVILEGE_SET structure [Security], SE_PRIVILEGE_ENABLED, SE_PRIVILEGE_ENABLED_BY_DEFAULT, SE_PRIVILEGE_USED_FOR_ACCESS, _PRIVILEGE_SET, _win32_privilege_set_str, security.privilege_set, winnt/PPRIVILEGE_SET, winnt/PRIVILEGE_SET"
ms.topic: struct
req.header: winnt.h
req.include-header: Windows.h
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
 - Winnt.h
api_name:
 - PRIVILEGE_SET
product: Windows
targetos: Windows
req.typenames: PRIVILEGE_SET, *PPRIVILEGE_SET
req.redist: 
---

# PRIVILEGE_SET structure


## -description


The <b>PRIVILEGE_SET</b> structure specifies a set of <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">privileges</a>. It is also used to indicate which, if any, privileges are held by a user or group requesting access to an object.


## -struct-fields




### -field PrivilegeCount

Specifies the number of privileges in the privilege set.


### -field Control

Specifies a control flag related to the privileges. The PRIVILEGE_SET_ALL_NECESSARY control flag is currently defined. It indicates that all of the specified privileges must be held by the <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">process</a> requesting access. If this flag is not set, the presence of any privileges in the user's <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">access token</a> grants the access.


### -field Privilege

Specifies an array of 
<a href="https://msdn.microsoft.com/f337b561-4b67-42a0-b8de-06f546bafb26">LUID_AND_ATTRIBUTES</a> structures describing the set's privileges. The following attributes are defined for privileges. 




					

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="SE_PRIVILEGE_ENABLED_BY_DEFAULT"></a><a id="se_privilege_enabled_by_default"></a><dl>
<dt><b>SE_PRIVILEGE_ENABLED_BY_DEFAULT</b></dt>
</dl>
</td>
<td width="60%">
The privilege is enabled by default.

</td>
</tr>
<tr>
<td width="40%"><a id="SE_PRIVILEGE_ENABLED"></a><a id="se_privilege_enabled"></a><dl>
<dt><b>SE_PRIVILEGE_ENABLED</b></dt>
</dl>
</td>
<td width="60%">
The privilege is enabled.

</td>
</tr>
<tr>
<td width="40%"><a id="SE_PRIVILEGE_USED_FOR_ACCESS"></a><a id="se_privilege_used_for_access"></a><dl>
<dt><b>SE_PRIVILEGE_USED_FOR_ACCESS</b></dt>
</dl>
</td>
<td width="60%">
The privilege was used to gain access to an object or service. This flag is used to identify the relevant privileges in a set passed by a client application that may contain unnecessary privileges.

</td>
</tr>
</table>
 


## -remarks



A privilege is used to control access to an object or service more strictly than is typical with discretionary access control. A system manager uses privileges to control which users are able to manipulate system resources. An application uses privileges when it changes a system-wide resource, such as when it changes the system time or shuts down the system.




## -see-also




<a href="https://msdn.microsoft.com/a812a46b-f23f-45b1-a6c6-48f931b78750">LUID</a>



<a href="https://msdn.microsoft.com/f337b561-4b67-42a0-b8de-06f546bafb26">LUID_AND_ATTRIBUTES</a>



<a href="https://msdn.microsoft.com/a73d934a-1abf-4e60-bf0a-6c4629f28f7a">PrivilegeCheck</a>
 

 

