---
UID: NF:clusapi.ClusterRegCloseReadBatchReply
title: ClusterRegCloseReadBatchReply function
author: windows-sdk-content
description: Closes a read batch result handle and frees the memory associated with it.
old-location: mscs\clusterregclosereadbatchreply.htm
tech.root: MsCS
ms.assetid: C8CC4292-A7CC-4613-B5A8-B504E804E00E
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClusterRegCloseReadBatchReply, ClusterRegCloseReadBatchReply function [Failover Cluster], clusapi/ClusterRegCloseReadBatchReply, mscs.clusterregclosereadbatchreply
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
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
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-0.dll
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-1.dll
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-2.dll
api_name:
 - ClusterRegCloseReadBatchReply
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterRegCloseReadBatchReply function


## -description


Closes a read batch result handle and frees the memory associated with it.


## -parameters




### -param hRegReadBatchReply [in]

A handle to a read batch result that was created by calling the <a href="https://msdn.microsoft.com/A164EB9F-290E-446E-98E9-95C6C3C3D00C">ClusterRegCloseReadBatch</a> function.


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
<dt><b>ERROR_INVALID_HANDLE</b></dt>
<dt>6</dt>
</dl>
</td>
<td width="60%">
<i>hRegReadBatchReply</i> is <b>NULL</b> or not valid.

</td>
</tr>
</table>
 




## -remarks



Call the <b>ClusterRegCloseReadBatchReply</b> function to close a read batch result that was created by the  <a href="https://msdn.microsoft.com/A164EB9F-290E-446E-98E9-95C6C3C3D00C">ClusterRegCloseReadBatch</a> function.




## -see-also




<a href="https://msdn.microsoft.com/A164EB9F-290E-446E-98E9-95C6C3C3D00C">ClusterRegCloseReadBatch</a>



<a href="https://msdn.microsoft.com/4E0DEB5C-36AA-480C-913C-235DE9AEA58D">ClusterRegReadBatchReplyNextCommand</a>
 

 

