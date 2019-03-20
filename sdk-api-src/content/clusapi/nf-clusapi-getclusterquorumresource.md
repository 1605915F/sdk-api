---
UID: NF:clusapi.GetClusterQuorumResource
title: GetClusterQuorumResource function (clusapi.h)
author: windows-sdk-content
description: Returns the name of a cluster's quorum resource.
old-location: mscs\getclusterquorumresource.htm
tech.root: MsCS
ms.assetid: 0f841070-9dc0-49e0-9112-8d46185470b5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetClusterQuorumResource, GetClusterQuorumResource function [Failover Cluster], PCLUSAPI_GET_CLUSTER_QUORUM_RESOURCE, PCLUSAPI_GET_CLUSTER_QUORUM_RESOURCE function [Failover Cluster], _wolf_getclusterquorumresource, clusapi/GetClusterQuorumResource, clusapi/PCLUSAPI_GET_CLUSTER_QUORUM_RESOURCE, mscs.getclusterquorumresource
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Enterprise, Windows Server 2008 Datacenter
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
 - GetClusterQuorumResource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetClusterQuorumResource function


## -description


Returns the name of a cluster's  <a href="https://msdn.microsoft.com/4c2ee30e-4de2-44ba-93ba-d2d89196545e">quorum resource</a>. The <b>PCLUSAPI_GET_CLUSTER_QUORUM_RESOURCE</b> type defines a pointer to this function.


## -parameters




### -param hCluster [in]

Handle to an existing <a href="https://msdn.microsoft.com/en-us/library/Aa369336(v=VS.85).aspx">cluster</a>.


### -param lpszResourceName [out]

Pointer to a null-terminated Unicode string containing the name of the cluster's quorum resource. The name is read from the quorum resource's  <a href="https://msdn.microsoft.com/61a4a2bc-e18f-4fac-82f0-8d5ef58e8d70">Name</a> common property. Do not pass <b>NULL</b> for this parameter.


### -param lpcchResourceName [in, out]

Pointer to the size of the <i>lpszResourceName</i> buffer as a count of characters. On input, specify the maximum number of characters the buffer can hold, including the terminating <b>NULL</b>. On output, specifies the number of characters in the resulting name, excluding the terminating <b>NULL</b>.


### -param lpszDeviceName [out]

Pointer to a null-terminated Unicode string containing the path to the location of the quorum log files maintained by the  <a href="https://msdn.microsoft.com/90717d6e-f2a4-49a0-86b6-17de1c4bcfe4">Cluster service</a>. Do not pass <b>NULL</b> for this parameter.


### -param lpcchDeviceName [in, out]

Pointer to the size of the <i>lpszDeviceName</i> buffer as a count of characters. On input, specify the maximum number of characters the buffer can hold, including the terminating <b>NULL</b>. On output, specifies the number of characters in the resulting name, excluding the terminating <b>NULL</b>.


### -param lpdwMaxQuorumLogSize [out]

Pointer to the maximum size (in bytes) of the log being maintained by the quorum resource. Do not pass <b>NULL</b> for this parameter.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>. The following is one of the possible values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_MORE_DATA</b></dt>
</dl>
</td>
<td width="60%">
The <i>lpszResourceName</i> or the <i>lpszDeviceName</i> buffer is not big enough to hold the result. The <i>lpcchResourceName</i> and <i>lpcchDeviceName</i> parameters return the number of characters in the result, excluding the terminating <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



Note that <i>lpcchName</i> refers to a count of characters and not a count of bytes, and that the returned size does not include the terminating <b>NULL</b> in the count. For more information on sizing buffers, see  <a href="https://msdn.microsoft.com/283dc560-d547-4b42-b45c-435045080639">Data Size Conventions</a>.




## -see-also




<a href="https://msdn.microsoft.com/61a4a2bc-e18f-4fac-82f0-8d5ef58e8d70">Name</a>



<a href="https://msdn.microsoft.com/1a00c09e-4470-4c02-807d-c559fd992066">SetClusterQuorumResource</a>
 

 

