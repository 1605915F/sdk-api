---
UID: NS:winnt._SYSTEM_SCOPED_POLICY_ID_ACE
title: SYSTEM_SCOPED_POLICY_ID_ACE
author: windows-sdk-content
description: Defines an access control entry (ACE) for the system access control list (SACL) that specifies the scoped policy identifier for a securable object.
old-location: security\system_scoped_policy_id_ace.htm
tech.root: secauthz
ms.assetid: 6B678A48-E024-4C67-A60C-5224868C04A5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSYSTEM_SCOPED_POLICY_ID_ACE, PSYSTEM_SCOPED_POLICY_ID_ACE, PSYSTEM_SCOPED_POLICY_ID_ACE structure pointer [Security], SYSTEM_SCOPED_POLICY_ID_ACE, SYSTEM_SCOPED_POLICY_ID_ACE structure [Security], _SYSTEM_SCOPED_POLICY_ID_ACE, security.system_scoped_policy_id_ace, winnt/PSYSTEM_SCOPED_POLICY_ID_ACE, winnt/SYSTEM_SCOPED_POLICY_ID_ACE"
ms.topic: struct
req.header: winnt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - SYSTEM_SCOPED_POLICY_ID_ACE
product: Windows
targetos: Windows
req.typenames: SYSTEM_SCOPED_POLICY_ID_ACE, *PSYSTEM_SCOPED_POLICY_ID_ACE
req.redist: 
---

# SYSTEM_SCOPED_POLICY_ID_ACE structure


## -description


The <b>SYSTEM_SCOPED_POLICY_ID_ACE</b> structure defines an <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">access control entry</a> (ACE) for the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">system access control list</a> (SACL) that specifies the scoped policy identifier for a securable object.


## -struct-fields




### -field Header

An <a href="https://msdn.microsoft.com/d23f15d6-0453-4aaf-a2db-7528b551a992">ACE_HEADER</a> structure that specifies the size and type of the ACE. The structure also contains flags that control inheritance of the ACE by child objects. The <b>AceType</b> member of the <b>ACE_HEADER</b> structure must be set to <b>SYSTEM_SCOPED_POLICY_ID_ACE</b>, and the <b>AceSize</b> member must be set to the total number of bytes allocated for the <b>SYSTEM_SCOPED_POLICY_ID_ACE</b> structure.


### -field Mask

The access policy associated with the SACL that contains this ACE.


### -field SidStart

Specifies the first <b>DWORD</b> of a <a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">SID</a>. 

