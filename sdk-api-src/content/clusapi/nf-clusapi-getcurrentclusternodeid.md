---
UID: NF:clusapi.GetCurrentClusterNodeId
title: GetCurrentClusterNodeId macro
author: windows-sdk-content
description: Returns the unique identifier of the current cluster node.
old-location: mscs\getcurrentclusternodeid.htm
tech.root: mscs
ms.assetid: 289abaaa-d063-4e99-91e7-441c58f7f75c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCurrentClusterNodeId, GetCurrentClusterNodeId macro [Failover Cluster], clusapi/GetCurrentClusterNodeId, mscs.getcurrentclusternodeid
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: macro
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ClusAPI.h
api_name:
 - GetCurrentClusterNodeId
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetCurrentClusterNodeId macro


## -description


Returns the unique identifier of the current cluster 
    <a href="https://msdn.microsoft.com/en-us/library/Aa371745(v=VS.85).aspx">node</a>.


## -parameters




#### - _lpszNodeId_ [out]

This parameter points to a buffer that receives the unique ID of <i>hNode</i>, including 
       the terminating <b>NULL</b> character.


#### - _lpcchName_ [in, out]

On input, pointer to the count of characters in the buffer pointed to by the 
       <i>lpszNodeId</i> parameter, including the <b>NULL</b> terminator. On 
       output, pointer to the count of characters stored in the buffer excluding the <b>NULL</b> 
       terminator.


#### - lpcchName [in, out]

On input, pointer to the count of characters in the buffer pointed to by the 
       <i>lpszNodeId</i> parameter, including the <b>NULL</b> terminator. On 
       output, pointer to the count of characters stored in the buffer excluding the <b>NULL</b> 
       terminator.


#### - lpszNodeId [out]

This parameter points to a buffer that receives the unique ID of <i>hNode</i>, including 
       the terminating <b>NULL</b> character.


## -remarks



Note that <i>lpcchName</i> refers to a count of characters and not a count of bytes, and 
     that the returned size does not include the terminating <b>NULL</b> in the count. For more information on sizing 
     buffers, see <a href="https://msdn.microsoft.com/en-us/library/Aa369338(v=VS.85).aspx">Data Size Conventions</a>.




## -see-also




<a href="https://msdn.microsoft.com/976ca079-10f7-4e12-9033-07ea83e8c92a">GetClusterNodeId</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa371760(v=VS.85).aspx">Node Management Functions</a>



<a href="https://msdn.microsoft.com/7658a030-d4b2-407c-829f-61491b5907e6">OpenClusterNode</a>
 

 

