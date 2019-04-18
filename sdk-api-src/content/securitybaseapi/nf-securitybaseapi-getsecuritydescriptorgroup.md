---
UID: NF:securitybaseapi.GetSecurityDescriptorGroup
title: GetSecurityDescriptorGroup function (securitybaseapi.h)
author: windows-sdk-content
description: Retrieves the primary group information from a security descriptor.
old-location: security\getsecuritydescriptorgroup.htm
tech.root: SecAuthZ
ms.assetid: a920b49e-a4c2-4e49-b529-88c12205d995
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSecurityDescriptorGroup, GetSecurityDescriptorGroup function [Security], _win32_getsecuritydescriptorgroup, security.getsecuritydescriptorgroup, securitybaseapi/GetSecurityDescriptorGroup
ms.topic: function
req.header: securitybaseapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
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
 - API-MS-Win-DownLevel-AdvApi32-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-DownLevel-AdvApi32-l1-1-1.dll
 - API-MS-Win-Security-base-l1-1-0.dll
 - API-MS-Win-Security-base-l1-2-0.dll
 - MinKernelBase.dll
 - API-MS-Win-Security-Base-L1-2-1.dll
api_name:
 - GetSecurityDescriptorGroup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetSecurityDescriptorGroup function


## -description


The <b>GetSecurityDescriptorGroup</b> function retrieves the primary group information from a <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security descriptor</a>.


## -parameters




### -param pSecurityDescriptor [in]

A pointer to a 
<a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">SECURITY_DESCRIPTOR</a> structure whose primary group information the function retrieves.


### -param pGroup [out]

A pointer to a pointer to a 
<a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifier</a> (SID) that identifies the primary group when the function returns. If the security descriptor does not contain a primary group, the function sets the pointer pointed to by <i>pGroup</i> to <b>NULL</b> and ignores the remaining output parameter, <i>lpbGroupDefaulted</i>. If the security descriptor contains a primary group, the function sets the pointer pointed to by <i>pGroup</i> to the address of the security descriptor's group SID and provides a valid value for the variable pointed to by <i>lpbGroupDefaulted</i>.


### -param lpbGroupDefaulted [out]

A pointer to a flag that is set to the value of the SE_GROUP_DEFAULTED flag in the 
<a href="https://msdn.microsoft.com/9a4ef57e-c374-4ef6-99dc-1a8dd250f2c2">SECURITY_DESCRIPTOR_CONTROL</a> structure when the function returns. If the value stored in the variable pointed to by the <i>pGroup</i> parameter is <b>NULL</b>, no value is set.


## -returns



If the function succeeds, the function returns nonzero.

If the function fails, it returns zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -see-also




<a href="https://msdn.microsoft.com/d66682f2-8017-4245-9d93-5f8332a5b483">GetSecurityDescriptorControl</a>



<a href="https://msdn.microsoft.com/8006c8bb-4976-463f-b074-a59c3bbab36b">GetSecurityDescriptorDacl</a>



<a href="https://msdn.microsoft.com/eb331839-ff3e-4f4b-b93b-18da2ea72697">GetSecurityDescriptorLength</a>



<a href="https://msdn.microsoft.com/58e810db-348e-430c-a61f-79f67826b60d">GetSecurityDescriptorOwner</a>



<a href="https://msdn.microsoft.com/6bf59735-aaa3-4751-8c98-00cc197df4e5">GetSecurityDescriptorSacl</a>



<a href="https://msdn.microsoft.com/24a98229-11e4-45ef-988b-c2cf831275e7">IsValidSecurityDescriptor</a>



<a href="https://msdn.microsoft.com/16337b77-23c5-4b7a-a344-66a02ee0e8a8">Low-level Access Control</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa375742(v=VS.85).aspx">Low-level Access Control Functions</a>



<a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">SECURITY_DESCRIPTOR</a>



<a href="https://msdn.microsoft.com/9a4ef57e-c374-4ef6-99dc-1a8dd250f2c2">SECURITY_DESCRIPTOR_CONTROL</a>



<a href="https://msdn.microsoft.com/060c375c-a313-4fa2-8d85-cee9369c26a8">SetSecurityDescriptorGroup</a>
 

 

