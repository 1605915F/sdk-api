---
UID: NF:clusapi.ClusterRegCreateBatch
title: ClusterRegCreateBatch function
author: windows-sdk-content
description: Creates a batch that will execute commands on a cluster registry key.
old-location: mscs\clusterregcreatebatch.htm
tech.root: MsCS
ms.assetid: 83e7c216-f08f-4dc2-9b53-faa2760985d4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClusterRegCreateBatch, ClusterRegCreateBatch function [Failover Cluster], PCLUSTER_REG_CREATE_BATCH, clusapi/ClusterRegCreateBatch, mscs.clusterregcreatebatch
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ClusAPI.lib
req.dll: ClusAPI.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ClusAPI.dll
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-1.dll
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-2.dll
api_name:
 - ClusterRegCreateBatch
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterRegCreateBatch function


## -description


Creates a batch that will execute commands on a cluster registry key. These commands will 
    be added to the batch by the 
    <a href="https://msdn.microsoft.com/3d59e68a-deb3-443f-9d8f-281cdb15e8b6">ClusterRegBatchAddCommand</a> function and 
    either executed or ignored by the 
    <a href="https://msdn.microsoft.com/d43644cf-370b-499f-b321-24e43f145a98">ClusterRegCloseBatch</a> function.


## -parameters




### -param hKey [in, optional]

The handle of the opened cluster registry key.  All the operations on the batch are relative to this cluster 
       registry key.


### -param pHREGBATCH [out]

The pointer to the handle of the created batch.


## -returns



The function returns one of the following 
       <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The operation was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_OUTOFMEMORY</b></dt>
<dt>14 (0xE)</dt>
</dl>
</td>
<td width="60%">
Not enough storage is available to complete this operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_GEN_FAILURE</b></dt>
<dt>31 (0x1F)</dt>
</dl>
</td>
<td width="60%">
A device attached to the system is not functioning.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
<dt>87 (0x57)</dt>
</dl>
</td>
<td width="60%">
The parameter is incorrect. This value will be returned if the <i>hKey</i> parameter is 
         <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



The key should not be closed until the batch has been submitted for execution.

The <b>PCLUSTER_REG_CREATE_BATCH</b> type defines a pointer to this function.




## -see-also




<a href="https://msdn.microsoft.com/2bb0650f-ef9c-40bb-ae90-229bfa23838e">Cluster Registry Access Functions</a>



<a href="https://msdn.microsoft.com/3d59e68a-deb3-443f-9d8f-281cdb15e8b6">ClusterRegBatchAddCommand</a>



<a href="https://msdn.microsoft.com/d43644cf-370b-499f-b321-24e43f145a98">ClusterRegCloseBatch</a>
 

 

