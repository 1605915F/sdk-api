---
UID: NF:winsync.IKnowledgeSyncProvider.ProcessChangeBatch
title: IKnowledgeSyncProvider::ProcessChangeBatch (winsync.h)
author: windows-sdk-content
description: Processes a set of changes by detecting conflicts and applying changes to the item store.
old-location: winsync\iknowledgesyncprovider_processchangebatch.htm
tech.root: winsync
ms.assetid: 528a109a-9c11-4e20-b3d5-9bb7241d02b6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IKnowledgeSyncProvider interface [Windows Sync],ProcessChangeBatch method, IKnowledgeSyncProvider.ProcessChangeBatch, IKnowledgeSyncProvider::ProcessChangeBatch, ProcessChangeBatch, ProcessChangeBatch method [Windows Sync], ProcessChangeBatch method [Windows Sync],IKnowledgeSyncProvider interface, winsync.iknowledgesyncprovider_processchangebatch, winsync/IKnowledgeSyncProvider::ProcessChangeBatch
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
 - IKnowledgeSyncProvider.ProcessChangeBatch
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IKnowledgeSyncProvider::ProcessChangeBatch


## -description


Processes a set of changes by detecting conflicts and applying changes to the item store.


## -parameters




### -param resolutionPolicy [in]

The conflict resolution policy to use when this method applies changes.


### -param pSourceChangeBatch [in]

A batch of changes from the source provider to be applied locally.


### -param pUnkDataRetriever [in]

An object that can be used to retrieve change data. It can be an <a href="https://msdn.microsoft.com/d59a5198-5878-4a48-b6c4-042afc36054d">ISynchronousDataRetriever</a> object or a provider-specific object.


### -param pCallback [in]

An object that receives event notifications during change application.


### -param pSyncSessionStatistics [in, out]

Tracks change statistics. For a provider that uses custom change application, this object must be updated with the results of the change application.


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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Provider-determined error codes</b></dt>
</dl>
</td>
<td width="60%"></td>
</tr>
</table>
 




## -remarks



When a source change contains change unit changes, the destination provider must determine which, if any, change unit versions to include in the batch of destination versions that is sent to the change applier. This decision depends on the kind of change from the source provider and whether the item is marked as deleted on the destination replica.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd316936(v=VS.85).aspx">CONFLICT RESOLUTION POLICY Enumeration</a>



<a href="https://msdn.microsoft.com/396bbf7e-7fd0-4a2e-8304-f87097cd5e50">IKnowledgeSyncProvider Interface</a>
 

 

