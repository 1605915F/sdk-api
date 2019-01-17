---
UID: NF:clusapi.ClusterRegGetBatchNotification
title: ClusterRegGetBatchNotification function
author: windows-sdk-content
description: Fetches the batch notification.
old-location: mscs\clusterreggetbatchnotification.htm
tech.root: MsCS
ms.assetid: 4cc6925f-cf91-449b-8f9d-fcf48b4df896
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClusterRegGetBatchNotification, ClusterRegGetBatchNotification function [Failover Cluster], PCLUSTER_REG_GET_BATCH_NOTIFICATION, PCLUSTER_REG_GET_BATCH_NOTIFICATION function [Failover Cluster], clusapi/ClusterRegGetBatchNotification, clusapi/PCLUSTER_REG_GET_BATCH_NOTIFICATION, mscs.clusterreggetbatchnotification
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
api_name:
 - ClusterRegGetBatchNotification
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterRegGetBatchNotification function


## -description


Fetches the batch notification. After the batch notification has been fetched, it is 
    interpreted via the 
    <a href="https://msdn.microsoft.com/a1a7abc5-f306-4664-bb53-e54c6ee1051e">ClusterRegBatchReadCommand</a> function. After 
    the batch notification is processed, it needs to be closed via the 
    <a href="https://msdn.microsoft.com/d7a127ba-6e97-46ac-8510-2da355359c50">ClusterRegBatchCloseNotification</a> 
    function.


## -parameters




### -param hBatchNotify [in]

The handle to the batch notification port opened earlier via the 
       <a href="https://msdn.microsoft.com/1eca2ba5-c0c3-4388-9384-db9dbcfc8405">ClusterRegCreateBatchNotifyPort</a> 
       function.


### -param phBatchNotification [out]

A handle to the batch notification that represents all of the changes at or below the cluster registry key of 
       interest that have happened since the last call to 
       <b>ClusterRegGetBatchNotification</b> or 
       since the batch notification port was opened.


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
<dt><b>ERROR_INVALID_DATA</b></dt>
<dt>13 (0xD)</dt>
</dl>
</td>
<td width="60%">
The data is not valid.

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
</table>
 




## -remarks



The <b>PCLUSTER_REG_GET_BATCH_NOTIFICATION</b> type defines a pointer to this 
     function.

Only the functions from the batch function group, such as <a href="https://msdn.microsoft.com/3d59e68a-deb3-443f-9d8f-281cdb15e8b6">ClusterRegBatchAddCommand</a>,  will generate a registry change notification. A registry change that does not use one of the batch function commands will not generate a batch notification.




## -see-also




<a href="https://msdn.microsoft.com/2bb0650f-ef9c-40bb-ae90-229bfa23838e">Cluster Registry Access Functions</a>



<a href="https://msdn.microsoft.com/d7a127ba-6e97-46ac-8510-2da355359c50">ClusterRegBatchCloseNotification</a>



<a href="https://msdn.microsoft.com/a1a7abc5-f306-4664-bb53-e54c6ee1051e">ClusterRegBatchReadCommand</a>



<a href="https://msdn.microsoft.com/1eca2ba5-c0c3-4388-9384-db9dbcfc8405">ClusterRegCreateBatchNotifyPort</a>
 

 

