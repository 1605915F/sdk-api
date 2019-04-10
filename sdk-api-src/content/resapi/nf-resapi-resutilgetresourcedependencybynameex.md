---
UID: NF:resapi.ResUtilGetResourceDependencyByNameEx
title: ResUtilGetResourceDependencyByNameEx function (resapi.h)
author: windows-sdk-content
description: Enumerates the dependencies of a specified resource in a specified cluster and returns a handle to a dependency of a specified type. The PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_NAME_EX type defines a pointer to this function.
old-location: mscs\resutilgetresourcedependencybynameex.htm
tech.root: MsCS
ms.assetid: 3BB9E8D4-2E8C-4A67-966F-6E2729ACE9A9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_NAME, PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_NAME function [Failover Cluster], ResUtilGetResourceDependencyByNameEx, ResUtilGetResourceDependencyByNameEx function [Failover Cluster], mscs.resutilgetresourcedependencybynameex, resapi/PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_NAME, resapi/ResUtilGetResourceDependencyByNameEx
ms.topic: function
req.header: resapi.h
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
req.lib: ResUtils.lib
req.dll: ResUtils.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ResUtils.dll
api_name:
 - ResUtilGetResourceDependencyByNameEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilGetResourceDependencyByNameEx function


## -description


Enumerates the  <a href="https://msdn.microsoft.com/2ad913d2-99cb-4885-a1de-822f77dc2030">dependencies</a> of a specified  <a href="https://msdn.microsoft.com/090d1c20-fab3-43dd-bfe2-a2c3f9ba8f89">resource</a> in a specified <a href="https://msdn.microsoft.com/en-us/library/Aa369336(v=VS.85).aspx">cluster</a> and returns a handle to a dependency of a specified type. The <b>PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_NAME_EX</b> type defines a pointer to this function.


## -parameters




### -param hCluster [in]

A handle to the cluster to which the resource belongs.


### -param hSelf [in]

A handle to the dependent resource. This resource depends on one or more resources.


### -param lpszResourceType [in]

A null-terminated Unicode string that specifies  the resource type of the dependency to return.


### -param bRecurse [in]

Determines the scope of the search. If <b>TRUE</b>, the function checks the entire dependency tree under the dependent resource. If <b>FALSE</b>, the function checks only the resources on which the dependent resource directly depends.


### -param dwDesiredAccess [in]

The requested access privileges. This  might be any combination of <b>GENERIC_READ</b> (0x80000000), <b>GENERIC_ALL</b> (0x10000000), or <b>MAXIMUM_ALLOWED</b> (0x02000000). If this value is zero (0), an undefined error  might be returned. Using <b>GENERIC_ALL</b> is the same as calling <a href="https://msdn.microsoft.com/8c978b27-fd1a-47b6-8a30-cfe6e4fbcf57">ResUtilGetResourceDependencyByName</a>.


## -returns



If the operation succeeds, the function returns a handle to one of the resources on which the resource that is specified by <i>hSelf</i> depends. The caller is responsible for closing the handle by calling  <a href="https://msdn.microsoft.com/dbefd7f9-3499-45b3-a5c8-d0000632f61c">CloseClusterResource</a>.

If the operation fails, the function returns <b>NULL</b>. For more information, call the   <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>HRESOURCE</b></dt>
</dl>
</td>
<td width="60%"></td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>NULL</b></b></dt>
</dl>
</td>
<td width="60%">
The operation was not successful. For more information, call the function  <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/42eb7c1b-6bd6-4997-b33e-ed16470c8475">Resource Utility Functions</a>
 

 

