---
UID: NS:aclui._EFFPERM_RESULT_LIST
title: EFFPERM_RESULT_LIST
author: windows-sdk-content
description: Lists the effective permissions.
old-location: security\effperm_result_list.htm
tech.root: secauthz
ms.assetid: D83C5632-F67A-42BA-A146-989EBB3B2763
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PEFFPERM_RESULT_LIST, EFFPERM_RESULT_LIST, EFFPERM_RESULT_LIST structure [Security], PEFFPERM_RESULT_LIST, PEFFPERM_RESULT_LIST structure pointer [Security], aclui/EFFPERM_RESULT_LIST, aclui/PEFFPERM_RESULT_LIST, security.effperm_result_list"
ms.topic: struct
req.header: aclui.h
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
 - Aclui.h
api_name:
 - EFFPERM_RESULT_LIST
product: Windows
targetos: Windows
req.typenames: EFFPERM_RESULT_LIST, *PEFFPERM_RESULT_LIST
req.redist: 
---

# EFFPERM_RESULT_LIST structure


## -description


The <b>EFFPERM_RESULT_LIST</b> structure lists the effective permissions.


## -struct-fields




### -field fEvaluated

Indicates if the effective permissions results have been evaluated.


### -field cObjectTypeListLength

The number of elements in both the <b>pObjectTypeList</b> and <b>pGrantedAccessList</b> members.


### -field pObjectTypeList

A pointer to an array of <a href="https://msdn.microsoft.com/c729ff1a-65f3-4f6f-84dd-5700aead75ce">OBJECT_TYPE_LIST</a> structures that specifies the properties and property sets for which access was evaluated.


### -field pGrantedAccessList

A pointer to an array of <a href="https://msdn.microsoft.com/f115ee54-3333-4109-8004-d71904a7a943">ACCESS_MASK</a> values that specifies the access rights granted for each corresponding object type.

