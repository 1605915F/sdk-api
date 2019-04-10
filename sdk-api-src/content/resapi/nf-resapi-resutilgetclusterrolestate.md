---
UID: NF:resapi.ResUtilGetClusterRoleState
title: ResUtilGetClusterRoleState function (resapi.h)
author: windows-sdk-content
description: Determines whether or not a specific role has been assigned to a cluster.
old-location: mscs\resutilgetclusterrolestate.htm
tech.root: MsCS
ms.assetid: 582992ca-9381-4673-8fe8-835b50047f51
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ClusterRoleDHCP, ClusterRoleDTC, ClusterRoleFileServer, ClusterRoleGenericApplication, ClusterRoleGenericScript, ClusterRoleGenericService, ClusterRoleISCSINameServer, ClusterRoleMSMQ, ClusterRoleNFS, ClusterRolePrintServer, ClusterRoleStandAloneNamespaceServer, ClusterRoleVolumeShadowCopyServiceTask, ClusterRoleWINS, ResUtilGetClusterRoleState, ResUtilGetClusterRoleState function [Failover Cluster], mscs.resutilgetclusterrolestate, resapi/ResUtilGetClusterRoleState
ms.topic: function
req.header: resapi.h
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
req.lib: ResUtils.lib; ResApi.lib on Windows Server 2008 R2 and Windows Server 2008
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
 - ResUtilGetClusterRoleState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilGetClusterRoleState function


## -description


Determines whether or not a specific role has been assigned to a cluster.


## -parameters




### -param hCluster [in]

The handle of the queried cluster.


### -param eClusterRole [in]

The role the cluster was queried about.  The possible values for this parameter are enumerators from the <a href="https://msdn.microsoft.com/65fc8a8f-0a9e-464c-b62a-d2e61431d927">CLUSTER_ROLE</a> enumeration.  The following values are valid.



#### ClusterRoleDHCP (0)

This enumerator represents the DHCP Service cluster role.



#### ClusterRoleDTC (1)

This enumerator represents the Distributed Transaction Coordinator cluster role.



#### ClusterRoleFileServer (2)

This enumerator represents the File Share cluster role.



#### ClusterRoleGenericApplication (3)

This enumerator represents the Generic Application cluster role.



#### ClusterRoleGenericScript (4)

This enumerator represents the Generic Script cluster role.



#### ClusterRoleGenericService (5)

This enumerator represents the Generic Service cluster role.



#### ClusterRoleISCSINameServer (6)

This enumerator represents the Microsoft iSNS cluster role.



#### ClusterRoleMSMQ (7)

This enumerator represents the Microsoft Message Queue cluster role.



#### ClusterRoleNFS (8)

This enumerator represents the NFS Share cluster role.



#### ClusterRolePrintServer (9)

This enumerator represents the Print Spooler cluster role.



#### ClusterRoleStandAloneNamespaceServer (10)

This enumerator represents a specialized File Share cluster role.



#### ClusterRoleVolumeShadowCopyServiceTask (11)

This enumerator represents the Volume Shadow Copy Service Task cluster role.



#### ClusterRoleWINS (12)

This enumerator represents the WINS Service cluster role.


## -returns



The possible return values for this function are enumerators from the  <a href="https://msdn.microsoft.com/21424e31-4eba-4ff9-95c1-0908827936df">CLUSTER_ROLE_STATE</a> enumeration.  The following values are valid.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterRoleUnknown</b></dt>
<dt>-1</dt>
</dl>
</td>
<td width="60%">
It is unknown whether or not the role is clustered.  If this value is returned then an error has occurred.  For more information call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterRoleClustered</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The role is clustered.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterRoleUnclustered</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
The role is not clustered.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/65fc8a8f-0a9e-464c-b62a-d2e61431d927">CLUSTER_ROLE</a>



<a href="https://msdn.microsoft.com/21424e31-4eba-4ff9-95c1-0908827936df">CLUSTER_ROLE_STATE</a>



<a href="https://msdn.microsoft.com/42eb7c1b-6bd6-4997-b33e-ed16470c8475">Resource Utility Functions</a>
 

 

