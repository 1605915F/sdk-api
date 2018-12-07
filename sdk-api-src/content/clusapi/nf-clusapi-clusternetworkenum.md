---
UID: NF:clusapi.ClusterNetworkEnum
title: ClusterNetworkEnum function
author: windows-sdk-content
description: Enumerates cluster objects on a network, returning the name of one object with each call.
old-location: mscs\clusternetworkenum.htm
tech.root: mscs
ms.assetid: 41cfb436-7494-4065-b287-075c4c771278
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CLUSTER_NETWORK_ENUM_NETINTERFACES, ClusterNetworkEnum, ClusterNetworkEnum function [Failover Cluster], PCLUSAPI_CLUSTER_NETWORK_ENUM, PCLUSAPI_CLUSTER_NETWORK_ENUM function [Failover Cluster], _wolf_clusternetworkenum, clusapi/ClusterNetworkEnum, clusapi/PCLUSAPI_CLUSTER_NETWORK_ENUM, mscs.clusternetworkenum
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
api_name:
 - ClusterNetworkEnum
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterNetworkEnum function


## -description


Enumerates <a href="https://msdn.microsoft.com/en-us/library/Aa369115(v=VS.85).aspx">cluster objects</a> on a 
    <a href="https://msdn.microsoft.com/en-us/library/Aa371501(v=VS.85).aspx">network</a>, returning the name of one object with each call. The <b>PCLUSAPI_CLUSTER_NETWORK_ENUM</b> type defines a pointer to this function.


## -parameters




### -param hNetworkEnum [in]

A handle to an existing enumeration object originally returned by the 
       <a href="https://msdn.microsoft.com/59f6fd26-1d96-4b04-858d-bfd3e4d25d01">ClusterNetworkOpenEnum</a> function.


### -param dwIndex [in]

The index used to identify the next entry to be enumerated. This parameter should be zero for the first call 
       to <b>ClusterNetworkEnum</b> and then incremented for 
       subsequent calls.


### -param lpdwType [out]

A pointer to the type of object returned. The following value of the 
       <a href="https://msdn.microsoft.com/en-us/library/Bb309153(v=VS.85).aspx">CLUSTER_NETWORK_ENUM</a> enumeration is returned with 
       each call.



#### CLUSTER_NETWORK_ENUM_NETINTERFACES (1)

The object is a <a href="https://msdn.microsoft.com/en-us/library/Aa371519(v=VS.85).aspx">network interface</a>.


### -param lpszName [out]

A pointer to a null-terminated Unicode string containing the name of the returned object.


### -param lpcchName [in, out]

A pointer to the size of the <i>lpszName</i> buffer as a count of characters. On input, 
       specify the maximum number of characters the buffer can hold, including the terminating 
       <b>NULL</b>. On output, specifies the number of characters in the resulting name, excluding 
       the terminating <b>NULL</b>.


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
The operation completed successfully.

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
More data is available. This value is returned if the buffer pointed to by 
         <i>lpszName</i> is not big enough to hold the result. The 
         <i>lpcchName</i> parameter returns the number of characters in the result, excluding the 
         terminating <b>NULL</b>.

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
No more data is available. This value is returned if there are no more objects of the requested type to be 
         returned.

</td>
</tr>
</table>
 




## -remarks



The <b>ClusterNetworkEnum</b> function is typically 
     used to iterate through a collection of objects of one or more types belonging to a network object. If, for 
     example, an application wants to enumerate all of the 
     <a href="https://msdn.microsoft.com/en-us/library/Aa371519(v=VS.85).aspx">network interface</a> objects on a network, it 
     calls <a href="https://msdn.microsoft.com/59f6fd26-1d96-4b04-858d-bfd3e4d25d01">ClusterNetworkOpenEnum</a> to 
     open a network enumerator that can process network interface objects. The <i>dwType</i> 
     parameter is set to <b>CLUSTER_NETWORK_ENUM_NETINTERFACES</b> to specify network interfaces 
     as the object type to be enumerated. With the handle that 
     <a href="https://msdn.microsoft.com/59f6fd26-1d96-4b04-858d-bfd3e4d25d01">ClusterNetworkOpenEnum</a> returns, 
     the application calls <b>ClusterNetworkEnum</b> 
     repeatedly to retrieve each of the objects. The <i>lpdwType</i> parameter points to the type 
     of object that is retrieved.

Note that <i>lpcchName</i> refers to a count of characters and not a count of bytes, and 
     that the returned size does not include the terminating <b>NULL</b> in the count. For more 
     information on sizing buffers, see 
     <a href="https://msdn.microsoft.com/en-us/library/Aa369338(v=VS.85).aspx">Data Size Conventions</a>.


#### Examples

See <a href="https://msdn.microsoft.com/en-us/library/Aa369563(v=VS.85).aspx">Enumerating Objects</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb309153(v=VS.85).aspx">CLUSTER_NETWORK_ENUM</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa371731(v=VS.85).aspx">Cluster Network Management Functions</a>



<a href="https://msdn.microsoft.com/725164c5-dc6d-42f4-a703-06336711e72e">ClusterNetworkCloseEnum</a>



<a href="https://msdn.microsoft.com/59f6fd26-1d96-4b04-858d-bfd3e4d25d01">ClusterNetworkOpenEnum</a>
 

 

