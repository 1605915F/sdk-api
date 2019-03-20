---
UID: NF:winsync.ISyncKnowledge.ContainsChangeUnit
title: ISyncKnowledge::ContainsChangeUnit (winsync.h)
author: windows-sdk-content
description: Indicates whether the specified change unit change is known by this knowledge.
old-location: winsync\isyncknowledge_containschangeunit.htm
tech.root: winsync
ms.assetid: 67fc3b59-ad82-47a4-9fc6-2d980b9e26fe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ContainsChangeUnit, ContainsChangeUnit method [Windows Sync], ContainsChangeUnit method [Windows Sync],ISyncKnowledge interface, ISyncKnowledge interface [Windows Sync],ContainsChangeUnit method, ISyncKnowledge.ContainsChangeUnit, ISyncKnowledge::ContainsChangeUnit, winsync.isyncknowledge_containschangeunit, winsync/ISyncKnowledge::ContainsChangeUnit
ms.topic: method
req.header: winsync.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - COM
api_location:
 - winsync.h
api_name:
 - ISyncKnowledge.ContainsChangeUnit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISyncKnowledge::ContainsChangeUnit


## -description


Indicates whether the specified change unit change is known by this knowledge.


## -parameters




### -param pbVersionOwnerReplicaId [in]

The ID of the replica that originated the change unit change.


### -param pbItemId [in]

The ID of the item that contains the change unit to look up.


### -param pbChangeUnitId [in]

 The ID of the change unit to look up.


### -param pSyncVersion [in]

The version of the change unit change to look up.


## -returns



The possible return codes include, but are not limited to, the values shown in the following table.

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
The specified change unit change is contained in the knowledge.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The specified change unit change is not contained in the knowledge.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%"></td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/cfb08476-7b5d-4953-b723-5160330e57be">ISyncKnowledge Interface</a>



<a href="https://msdn.microsoft.com/6a493a58-3dab-4032-90de-be9f903ae489">SYNC_VERSION Structure</a>
 

 

