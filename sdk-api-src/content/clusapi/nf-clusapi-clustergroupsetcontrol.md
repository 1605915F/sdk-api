---
UID: NF:clusapi.ClusterGroupSetControl
title: ClusterGroupSetControl function
author: windows-sdk-content
description: Initiates an operation affecting a groupset.
old-location: mscs\clustergroupcollectioncontrol.htm
tech.root: MsCS
ms.assetid: 20f0f70a-b300-41b8-b215-e5a3f24db44b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClusterGroupSetControl, ClusterGroupSetControl function [Failover Cluster], PCLUSAPI_CLUSTER_GROUP_GROUPSET_CONTROL, PCLUSAPI_CLUSTER_GROUP_GROUPSET_CONTROL function [Failover Cluster], clusapi/ClusterGroupSetControl, clusapi/PCLUSAPI_CLUSTER_GROUP_GROUPSET_CONTROL, mscs.clustergroupcollectioncontrol
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2016
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
 - ClusterGroupSetControl
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterGroupSetControl function


## -description


Initiates an operation affecting a groupset.

The 
    operation performed depends on the <a href="https://msdn.microsoft.com/47618915-0985-4415-b7d4-5959fb27eb9f">control code</a> passed to the 
    <i>dwControlCode</i> parameter.


## -parameters




### -param hGroupSet [in]

Handle to the groupset to be affected.


### -param hHostNode [in, optional]

If non-<b>NULL</b>, handle to the node to perform the operation represented by the control 
       code. If <b>NULL</b>, the <a href="https://msdn.microsoft.com/4381e378-7bf2-4dbc-b56e-3fed33193d32">node</a> that owns the 
       groupset performs the operation. Specifying <i>hHostNode</i> is optional.


### -param dwControlCode [in]

A <a href="https://msdn.microsoft.com/85DD2E41-B5DA-41E8-ACD8-2BE283CCF67A">Collection Control Code</a> specifying 
       the operation to be performed. For the syntax associated with a control code, refer to  
       <a href="https://msdn.microsoft.com/d107f743-8ce8-4c0c-b7a2-24a70ffbc0f3">Control Code Architecture</a> and the following 
       topics.

<ul>
<li>
<a href="https://msdn.microsoft.com/CC8D848F-645B-4B26-8E70-DED95F25681B">CLUSCTL_GROUPSET_GET_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://msdn.microsoft.com/96C75F3B-F9E6-4557-BF41-C8F9D1E1EE3A">CLUSCTL_GROUPSET_GET_GROUPS</a>
</li>
<li>
<a href="https://msdn.microsoft.com/8C2AE592-67C9-4E57-B762-A95759F28538">CLUSCTL_GROUPSET_GET_PROVIDER_GROUPS</a>
</li>
<li>
<a href="https://msdn.microsoft.com/76222551-F27D-4354-8B4B-C9FA5EE55C22">CLUSCTL_GROUPSET_GET_PROVIDER_COLLECTIONS</a>
</li>
<li>
<a href="https://msdn.microsoft.com/F3410FAC-2FC0-4C59-BCB1-DED4DD63D5D8">CLUSCTL_GROUPSET_GET_RO_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://msdn.microsoft.com/B2C0D9C6-C26E-4A56-A15E-243ED6429C8E">CLUSCTL_GROUPSET_SET_COMMON_PROPERTIES</a>
</li>
<li>
<a href="https://msdn.microsoft.com/63347D0A-3C5B-4BC6-BE64-79E40D115F7B">CLUSCTL_GROUP_GET_PROVIDER_GROUPS</a>
</li>
<li>
<a href="https://msdn.microsoft.com/C51FDDBC-5E32-4950-9A1E-64843F184172">CLUSCTL_GROUP_GET_PROVIDER_COLLECTIONS</a>
</li>
</ul>

### -param lpInBuffer [in, optional]

Pointer to an input buffer containing information needed for the operation, or <b>NULL</b> 
       if no information is needed.


### -param cbInBufferSize [in]

The allocated size (in bytes) of the input buffer.


### -param lpOutBuffer [out, optional]

Pointer to an output buffer to receive the data resulting from the operation, or 
       <b>NULL</b> if no data will be returned.


### -param cbOutBufferSize [in]

The allocated size (in bytes) of the output buffer.


### -param lpBytesReturned [out, optional]

Returns the actual size (in bytes) of the data resulting from the operation. If this information is not 
       needed, pass <b>NULL</b> for <i>lpBytesReturned</i>.


## -returns



The function returns one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
The operation was successful. If the operation required an output buffer, 
         <i>lpBytesReturned</i> (if not <b>NULL</b> on input) points to the 
         actual size of the data returned in the buffer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_MORE_DATA</b></dt>
</dl>
</td>
<td width="60%">
The output buffer pointed to by <i>lpOutBuffer</i> was not large enough to hold the data 
         resulting from the operation. The <i>lpBytesReturned</i> parameter (if not 
         <b>NULL</b> on input) points to the size required for the output buffer. Only operations 
         requiring an output buffer return <b>ERROR_MORE_DATA</b>. If the 
         <i>lpOutBuffer</i> parameter is <b>NULL</b> and the 
         <i>nOutBufferSize</i> parameter is zero, then <b>ERROR_SUCCESS</b> may 
         be returned, not <b>ERROR_MORE_DATA</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System error code</a></b></dt>
</dl>
</td>
<td width="60%">
The operation was not successful. If the operation required an output buffer, the value specified by 
         <i>lpBytesReturned</i> (if not <b>NULL</b> on input) is 
         unreliable.

</td>
</tr>
</table>
 



