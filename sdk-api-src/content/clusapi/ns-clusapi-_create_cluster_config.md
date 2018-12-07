---
UID: NS:clusapi._CREATE_CLUSTER_CONFIG
title: "_CREATE_CLUSTER_CONFIG"
author: windows-sdk-content
description: Defines the initial cluster configuration.
old-location: mscs\create_cluster_config.htm
tech.root: mscs
ms.assetid: 5fc90422-47e4-44da-a49f-66d4b7712f53
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCREATE_CLUSTER_CONFIG, CREATE_CLUSTER_CONFIG, CREATE_CLUSTER_CONFIG structure [Failover Cluster], PCREATE_CLUSTER_CONFIG, PCREATE_CLUSTER_CONFIG structure pointer [Failover Cluster], _CREATE_CLUSTER_CONFIG, clusapi/CREATE_CLUSTER_CONFIG, clusapi/PCREATE_CLUSTER_CONFIG, mscs.create_cluster_config"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
 - CREATE_CLUSTER_CONFIG
product: Windows
targetos: Windows
req.typenames: CREATE_CLUSTER_CONFIG, *PCREATE_CLUSTER_CONFIG
req.redist: 
---

# _CREATE_CLUSTER_CONFIG structure


## -description


Defines the initial cluster configuration. This structure is passed in the 
    <i>pConfig</i> parameter to the 
    <a href="https://msdn.microsoft.com/672a1573-63e5-4321-a049-25bdafc1b5e0">CreateCluster</a> function.


## -struct-fields




### -field dwVersion

Version. Set this to <b>CLUSAPI_VERSION</b>.


### -field lpszClusterName

Name of the cluster.


### -field cNodes

Count of nodes in the array pointed to by the <b>ppszNodeNames</b> member.


### -field ppszNodeNames

Address of array of pointers to strings, each naming a node to be added to the new cluster.


### -field cIpEntries

Count of nodes in the array pointed to by the <b>pIpEntries</b> member. If zero (0), no 
       <a href="https://msdn.microsoft.com/en-us/library/Aa370484(v=VS.85).aspx">IP Address</a> or 
       <a href="https://msdn.microsoft.com/en-us/library/Aa371733(v=VS.85).aspx">Network Name</a> resources will be created.


### -field pIpEntries

Address of array of pointers to <a href="https://msdn.microsoft.com/en-us/library/Bb309151(v=VS.85).aspx">CLUSTER_IP_ENTRY</a> 
       structures, each naming a node to be added to the new cluster. Each entry will be used to configure a separate 
       <a href="https://msdn.microsoft.com/en-us/library/Aa370484(v=VS.85).aspx">IP Address</a> resource, and a 
       <a href="https://msdn.microsoft.com/en-us/library/Aa371733(v=VS.85).aspx">Network Name</a> resource will be created which 
       <a href="https://msdn.microsoft.com/en-us/library/Aa372236(v=VS.85).aspx">depends</a> on all of these 
       <a href="https://msdn.microsoft.com/en-us/library/Aa370484(v=VS.85).aspx">IP Address</a> resources in a logical 
       <b>OR</b> manner.


### -field fEmptyCluster

If <b>TRUE</b>, then the cluster is to be created without any nodes and the 
       <b>cIpEntries</b> member must be zero (0) and the <b>pIpEntries</b> 
       member must be <b>NULL</b>.

If <b>FALSE</b>, then the cluster is to be created with at least one node and the 
       <b>cIpEntries</b> member must be one (1) or more, the 
       <b>pIpEntries</b> member must not be <b>NULL</b>, the 
       <b>cNodes</b> member must be one (1) or more, the <b>ppszNodeNames</b> 
       member must not be <b>NULL</b>, and the <b>lpszClusterName</b> member 
       must not be <b>NULL</b>.


### -field managementPointType

A <a href="https://msdn.microsoft.com/en-us/library/Dn441155(v=VS.85).aspx">CLUSTER_MGMT_POINT_TYPE</a> value that specifies the management point type. If the value of the <b>fEmptyCluster</b> member of this structure is TRUE, this member is ignored and the structure is treated as if this member were set to <b>CLUSTER_MGMT_POINT_TYPE_NONE</b>. If the <b>dwVersion</b> member of this structure is set to a value less than <b>CLUSAPI_VERSION_WINDOWSBLUE</b>, the value of this member is ignored and the structure is treated as if this member were set to <b>CLUSTER_MGMT_POINT_TYPE_CNO</b>.

<b>Windows Server 2012, Windows Server 2008 R2 and Windows Server 2008:  </b>This member is not supported before Windows Server 2012 R2.


### -field managementPointResType

 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb309151(v=VS.85).aspx">CLUSTER_IP_ENTRY</a>



<a href="https://msdn.microsoft.com/672a1573-63e5-4321-a049-25bdafc1b5e0">CreateCluster</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa373109(v=VS.85).aspx">Utility structures</a>
 

 

