---
UID: NS:winnt._ACCESS_ALLOWED_CALLBACK_ACE
title: ACCESS_ALLOWED_CALLBACK_ACE
author: windows-sdk-content
description: The ACCESS_ALLOWED_CALLBACK_ACE structure defines an access control entry for the discretionary access control list that controls access to an object.
old-location: security\access_allowed_callback_ace.htm
tech.root: SecAuthZ
ms.assetid: 0dbca19b-4b54-4c55-920a-c00335692d68
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PACCESS_ALLOWED_CALLBACK_ACE, ACCESS_ALLOWED_CALLBACK_ACE, ACCESS_ALLOWED_CALLBACK_ACE structure [Security], PACCESS_ALLOWED_CALLBACK_ACE, PACCESS_ALLOWED_CALLBACK_ACE structure pointer [Security], _ACCESS_ALLOWED_CALLBACK_ACE, security.access_allowed_callback_ace, winnt/ACCESS_ALLOWED_CALLBACK_ACE, winnt/PACCESS_ALLOWED_CALLBACK_ACE"
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
 - ACCESS_ALLOWED_CALLBACK_ACE
product: Windows
targetos: Windows
req.typenames: ACCESS_ALLOWED_CALLBACK_ACE, *PACCESS_ALLOWED_CALLBACK_ACE
req.redist: 
---

# ACCESS_ALLOWED_CALLBACK_ACE structure


## -description


The <b>ACCESS_ALLOWED_CALLBACK_ACE</b> 
   structure defines an  <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">access control entry</a> 
   (ACE) for the  <a href="https://msdn.microsoft.com/d007cbb9-b547-4dc7-bc22-b526f650f7c2">discretionary access control list</a> (DACL) that controls access to an object. An access-allowed ACE allows access to an object for a specific 
   <a href="https://msdn.microsoft.com/11f2e098-1d1e-473b-90ff-7b86eb923e9f">trustee</a> identified by a  
   <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifier</a> (SID).
   

When the <a href="https://msdn.microsoft.com/633c2a73-169c-4e0c-abb6-96c360bd63cf">AuthzAccessCheck</a> 
   function is called, each 
   <b>ACCESS_ALLOWED_CALLBACK_ACE</b> structure contained in the DACL of a 
   <a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">SECURITY_DESCRIPTOR</a> structure passed through a pointer to the 
   <b>AuthzAccessCheck</b> function invokes a call to the application-defined 
   <a href="https://msdn.microsoft.com/e8a510e6-0739-4765-ad07-3bcb1b9c905c">AuthzAccessCheckCallback</a> function, in which a pointer to the 
   <b>ACCESS_ALLOWED_CALLBACK_ACE</b> structure found is passed in the 
   <i>pAce</i> parameter.


## -struct-fields




### -field Header


<a href="https://msdn.microsoft.com/d23f15d6-0453-4aaf-a2db-7528b551a992">ACE_HEADER</a> structure that specifies the size and type of ACE. It also contains flags that control inheritance of the ACE by child objects. The <b>AceType</b> member of the <b>ACE_HEADER</b> structure should be set to ACCESS_ALLOWED_CALLBACK_ACE_TYPE, and the <b>AceSize</b> member should be set to the total number of bytes allocated for the <b>ACCESS_ALLOWED_CALLBACK_ACE</b> structure.


### -field Mask

Specifies an 
<a href="https://msdn.microsoft.com/f115ee54-3333-4109-8004-d71904a7a943">ACCESS_MASK</a> structure that specifies the access rights granted by this ACE.


### -field SidStart

The first <b>DWORD</b> of a trustee's SID.


## -remarks



ACE structures must be aligned on <b>DWORD</b> boundaries. All Windows memory-management functions return <b>DWORD</b>-aligned handles to memory.

The access rights specified by the <b>Mask</b> member are granted to any <a href="https://msdn.microsoft.com/11f2e098-1d1e-473b-90ff-7b86eb923e9f">trustee</a> that possesses an enabled SID that matches the SID stored in the <b>SidStart</b> member.

When an <b>ACCESS_ALLOWED_CALLBACK_ACE</b> structure is created, sufficient memory must be allocated to accommodate the complete SID of the trustee in the <b>SidStart</b> member and the contiguous memory that follows it. 




## -see-also




<a href="https://msdn.microsoft.com/980b8242-2ba2-469f-b834-da7d3fb22e14">ACE</a>



<a href="https://msdn.microsoft.com/0073659f-c4d5-4aaf-aaa6-ea596d3bd8b9">ACL</a>



<a href="https://msdn.microsoft.com/be852a0c-9d96-4b29-b5f9-d9c41d838c12">AddAuditAccessObjectAce</a>



<a href="https://msdn.microsoft.com/323e33b7-676f-4ed0-a9c7-908273c6e10f">GUID</a>



<a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">SID</a>
 

 

