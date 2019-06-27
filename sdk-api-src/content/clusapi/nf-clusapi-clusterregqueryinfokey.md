---
UID: NF:clusapi.ClusterRegQueryInfoKey
title: ClusterRegQueryInfoKey function (clusapi.h)
author: windows-sdk-content
description: Returns information about a cluster database key.
old-location: mscs\clusterregqueryinfokey.htm
tech.root: MsCS
ms.assetid: 90feb6ae-bd15-4431-ba99-0116fa20e94a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ClusterRegQueryInfoKey, ClusterRegQueryInfoKey function [Failover Cluster], _wolf_clusterregqueryinfokey, clusapi/ClusterRegQueryInfoKey, mscs.clusterregqueryinfokey
ms.topic: function
f1_keywords: 
 - "clusapi/ClusterRegQueryInfoKey"
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
 - ClusterRegQueryInfoKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ClusterRegQueryInfoKey function


## -description


Returns information about a  <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mscs/cluster-database">cluster database</a> key.


## -parameters




### -param hKey [in]

Handle to a cluster database key. All subsequent parameters describe the contents of the key.


### -param lpcSubKeys [in]

If not <b>NULL</b>, pointer to the number of subkeys in the specified key.


### -param lpcchMaxSubKeyLen [in]

If not <b>NULL</b>, pointer to the number of characters in the longest subkey name in the specified key. The number does not include the terminating <b>NULL</b>.


### -param lpcValues [in]

If not <b>NULL</b>, pointer to the number of values in the specified key.


### -param lpcchMaxValueNameLen [in]

If not <b>NULL</b>, pointer to the number of characters in the longest value name in the specified key. The number does not include the terminating <b>NULL</b>.


### -param lpcbMaxValueLen [in]

If not <b>NULL</b>, pointer to the byte size of the largest data value in the specified key.


### -param lpcbSecurityDescriptor [in]

If not <b>NULL</b>, pointer to the byte size of the specified key's security descriptor.


### -param lpftLastWriteTime [in]

If not <b>NULL</b>, pointer to the time of the most recent modification to the specified key or any of its contents.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://docs.microsoft.com/windows/desktop/Debug/system-error-codes">system error code</a>.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/clusapi/nf-clusapi-clusterregopenkey">ClusterRegOpenKey</a>
 

 

