---
UID: NF:clusapi.ClusterRegBatchAddCommand
title: ClusterRegBatchAddCommand function (clusapi.h)
author: windows-sdk-content
description: Adds a command to a batch that will be executed on a cluster registry key.
old-location: mscs\clusterregbatchaddcommand.htm
tech.root: MsCS
ms.assetid: 3d59e68a-deb3-443f-9d8f-281cdb15e8b6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CLUSREG_CREATE_KEY, CLUSREG_DELETE_KEY, CLUSREG_DELETE_VALUE, CLUSREG_SET_VALUE, ClusterRegBatchAddCommand, ClusterRegBatchAddCommand function [Failover Cluster], PCLUSTER_REG_BATCH_ADD_COMMAND, clusapi/ClusterRegBatchAddCommand, mscs.clusterregbatchaddcommand
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
 - ClusterRegBatchAddCommand
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ClusterRegBatchAddCommand function


## -description


Adds a command to a batch that will be executed on a cluster registry key. Additional calls 
    to the function will yield additional commands added to the batch. The batch was created by the 
    <a href="https://msdn.microsoft.com/83e7c216-f08f-4dc2-9b53-faa2760985d4">ClusterRegCreateBatch</a> function and will be 
    either executed or ignored by the 
    <a href="https://msdn.microsoft.com/d43644cf-370b-499f-b321-24e43f145a98">ClusterRegCloseBatch</a> function.


## -parameters




### -param hRegBatch [in]

The handle of the batch to which a command will be added.


### -param dwCommand [in]

A command supported by this API that is taken from the 
       <a href="https://msdn.microsoft.com/1a1266dc-a223-48bd-be30-80c8b50c5b21">CLUSTER_REG_COMMAND</a> enumeration.  The possible 
       commands are as follows.



#### CLUSREG_SET_VALUE (1)

Sets a value relative to the last executed <b>CLUSREG_CREATE_KEY</b> command or (if 
         not provided) relative to a key passed into the 
         <a href="https://msdn.microsoft.com/83e7c216-f08f-4dc2-9b53-faa2760985d4">ClusterRegCreateBatch</a> function.



#### CLUSREG_CREATE_KEY (2)

Creates a specified cluster registry key if it does not exist, or opens an existing one.



#### CLUSREG_DELETE_KEY (3)

Deletes a key with all values and nested subkeys.  No commands that operate on values can follow 
         <b>CLUSREG_DELETE_KEY</b> until <b>CLUSREG_CREATE_KEY</b> is 
         added.



#### CLUSREG_DELETE_VALUE (4)

Deletes a value relative to the last executed <b>CLUSREG_CREATE_KEY</b> command or 
         (if not provided) relative to a key passed into  the 
         <a href="https://msdn.microsoft.com/83e7c216-f08f-4dc2-9b53-faa2760985d4">ClusterRegCreateBatch</a> function.


### -param wzName [in, optional]

The name of the value or key relative to the command issued by the <i>dwCommand</i> 
       parameter.


### -param dwOptions [in]

If <i>dwCommand</i> takes the <b>CLUSREG_SET_VALUE</b> command, then 
       this parameter takes one of the standard 
       <a href="https://msdn.microsoft.com/5fd828d6-4d62-4823-a2f1-15782b5cd28c">registry value types</a>. If not, then 
       <i>dwCommand</i> is set to 0.


### -param lpData [in, optional]

A pointer to the data relative to the command issued by <i>dwCommand</i>. The value of 
       this parameter is <b>NULL</b> for all but the <b>CLUSREG_SET_VALUE</b> 
       command.


### -param cbData [in]

The count, in bytes, of the data relative to the command issued by <i>dwCommand</i>. The 
       value of this parameter is 0 for all but the <b>CLUSREG_SET_VALUE</b> command.


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
<dt><b>ERROR_INVALID_FUNCTION</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
Incorrect function.  This value is returned if <i>dwCommand</i> takes any command other 
         than the commands described in the previous section.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_HANDLE</b></dt>
<dt>6</dt>
</dl>
</td>
<td width="60%">
The handle is not valid. This value is returned if the <i>hRegBatch</i> parameter is 
         <b>NULL</b>.

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
The parameter is incorrect. This value will be returned if the cluster registry key that the batch is 
         attempting to execute commands on is not the current key.

</td>
</tr>
</table>
 




## -remarks



The <b>PCLUSTER_REG_BATCH_ADD_COMMAND</b> type defines a pointer to this function.




## -see-also




<a href="https://msdn.microsoft.com/1a1266dc-a223-48bd-be30-80c8b50c5b21">CLUSTER_REG_COMMAND</a>



<a href="https://msdn.microsoft.com/2bb0650f-ef9c-40bb-ae90-229bfa23838e">Cluster Registry Access Functions</a>



<a href="https://msdn.microsoft.com/d43644cf-370b-499f-b321-24e43f145a98">ClusterRegCloseBatch</a>



<a href="https://msdn.microsoft.com/83e7c216-f08f-4dc2-9b53-faa2760985d4">ClusterRegCreateBatch</a>



<a href="https://msdn.microsoft.com/5fd828d6-4d62-4823-a2f1-15782b5cd28c">Registry Value Types</a>
 

 

