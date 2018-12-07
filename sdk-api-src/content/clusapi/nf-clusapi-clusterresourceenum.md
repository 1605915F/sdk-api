---
UID: NF:clusapi.ClusterResourceEnum
title: ClusterResourceEnum function
author: windows-sdk-content
description: Enumerates a resource's dependent resources, nodes, or both.
old-location: mscs\clusterresourceenum.htm
tech.root: mscs
ms.assetid: 73627594-90df-496d-8120-b24c34f13fb5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CLUSTER_RESOURCE_ENUM_DEPENDS, CLUSTER_RESOURCE_ENUM_NODES, CLUSTER_RESOURCE_ENUM_PROVIDES, ClusterResourceEnum, ClusterResourceEnum function [Failover Cluster], PCLUSAPI_CLUSTER_RESOURCE_ENUM, PCLUSAPI_CLUSTER_RESOURCE_ENUM function [Failover Cluster], _wolf_clusterresourceenum, clusapi/ClusterResourceEnum, clusapi/PCLUSAPI_CLUSTER_RESOURCE_ENUM, mscs.clusterresourceenum
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - Ext-MS-Win-Cluster-ClusAPI-L1-1-2.dll
api_name:
 - ClusterResourceEnum
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterResourceEnum function


## -description


Enumerates a <a href="https://msdn.microsoft.com/en-us/library/Aa372152(v=VS.85).aspx">resource's</a> dependent resources, 
    <a href="https://msdn.microsoft.com/en-us/library/Aa371745(v=VS.85).aspx">nodes</a>, or both. It returns the name of one 
    <a href="https://msdn.microsoft.com/en-us/library/Aa369115(v=VS.85).aspx">cluster object</a> with each call. The <b>PCLUSAPI_CLUSTER_RESOURCE_ENUM</b> type defines a pointer to this function.


## -parameters




### -param hResEnum [in]

A resource enumeration handle returned from 
       the <a href="https://msdn.microsoft.com/f801401f-f49d-41de-b88b-b832330eeccf">ClusterResourceOpenEnum</a> function.


### -param dwIndex [in]

The index of the resource or node object to return. This parameter should be zero for the first call to the 
       <b>ClusterResourceEnum</b> function and then 
       incremented for subsequent calls.


### -param lpdwType [out]

The type of object returned by 
       <b>ClusterResourceEnum</b>.


The possible values are one of the following <a href="https://msdn.microsoft.com/en-us/library/Bb309166(v=VS.85).aspx">CLUSTER_RESOURCE_ENUM</a> enumeration values:





#### CLUSTER_RESOURCE_ENUM_DEPENDS (1)

The object is a resource and  <i>hResEnum</i> is a resource that depends on this object.



#### CLUSTER_RESOURCE_ENUM_PROVIDES (2)

The object is a resource that depends on the resource identified by <i>hResEnum</i>.



#### CLUSTER_RESOURCE_ENUM_NODES (4)

The object is a node that can host the resource identified by <i>hResEnum</i>.


### -param lpszName [out]

A pointer to a null-terminated Unicode string containing the name of the returned object.


### -param lpcchName [in, out]

A pointer to the size of the <i>lpszName</i> buffer as a count of characters. On input, 
       specify the maximum number of characters the buffer can hold, including the terminating null character. On 
       output, specifies the number of characters in the resulting name, excluding the terminating null character.


## -returns



The function returns one of the following values.

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
The operation completed successfully or the <i>lpszName</i> parameter is 
         <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_MORE_DATA</b></dt>
<dt>234 (0xEA)</dt>
</dl>
</td>
<td width="60%">
The buffer pointed to by the <i>lpszName</i> parameter is not big enough to hold the 
         result. The <i>lpcchName</i> parameter returns the number of characters in the result, 
         excluding the terminating null character.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NO_MORE_ITEMS</b></dt>
<dt>259 (0x103)</dt>
</dl>
</td>
<td width="60%">
There are no more objects to be returned.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System error code</a></b></dt>
</dl>
</td>
<td width="60%">
Any other returned error code indicates that the operation failed.

</td>
</tr>
</table>
 




## -remarks



Note that <i>lpcchName</i> refers to a count of characters and not a count of bytes, and 
     that the returned size does not include the terminating null character in the count. For more information on 
     sizing buffers, see <a href="https://msdn.microsoft.com/en-us/library/Aa369338(v=VS.85).aspx">Data Size Conventions</a>.

Do not call <b>ClusterResourceEnum</b> from any 
     resource DLL entry point function. 
     <b>ClusterResourceEnum</b> can safely be called from a 
     worker thread. For more information, see 
     <a href="https://msdn.microsoft.com/en-us/library/Aa369588(v=VS.85).aspx">Function Calls to Avoid in Resource DLLs</a>.


#### Examples

See <a href="https://msdn.microsoft.com/en-us/library/Aa369563(v=VS.85).aspx">Enumerating Objects</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa372262(v=VS.85).aspx">Cluster Resource Management Functions</a>



<a href="https://msdn.microsoft.com/49407b45-2b7f-43a2-90ff-98cc557edb31">ClusterResourceCloseEnum</a>



<a href="https://msdn.microsoft.com/f801401f-f49d-41de-b88b-b832330eeccf">ClusterResourceOpenEnum</a>
 

 

