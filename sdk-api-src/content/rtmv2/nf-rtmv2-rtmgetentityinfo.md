---
UID: NF:rtmv2.RtmGetEntityInfo
title: RtmGetEntityInfo function
author: windows-sdk-content
description: The RtmGetEntityInfo function returns information about a previously registered client.
old-location: rras\rtmgetentityinfo.htm
tech.root: rras
ms.assetid: 6062369c-22c7-48e4-9dd3-91efba22df34
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: RtmGetEntityInfo, RtmGetEntityInfo function [RAS], _rtmv2ref_rtmgetentityinfo, rras.rtmgetentityinfo, rtmv2/RtmGetEntityInfo
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: rtmv2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Rtm.lib
req.dll: Rtm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Rtm.dll
api_name:
 - RtmGetEntityInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# RtmGetEntityInfo function


## -description


The 
<b>RtmGetEntityInfo</b> function returns information about a previously registered client.


## -parameters




### -param RtmRegHandle [in]

Handle to the client obtained from a previous call to 
<a href="https://msdn.microsoft.com/2b952ea2-cf33-49e3-ae31-a14b0907a1b5">RtmRegisterEntity</a>.


### -param EntityHandle [in]

Handle to the client for which to return information.


### -param EntityInfo [out]

On input, <i>EntityInfo</i> is a pointer to an 
<a href="https://msdn.microsoft.com/b2a1e6b9-0cac-4316-98a0-ff1d44c5a15a">RTM_ENTITY_INFO</a> structure. 




On output, <i>EntityInfo</i> receives the requested information.


## -returns



If the function succeeds, the return value is NO_ERROR.

If the function fails, the return value is one of the following error codes.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
The handle is invalid.

</td>
</tr>
</table>
 


<div> </div>





## -see-also




<a href="https://msdn.microsoft.com/b2a1e6b9-0cac-4316-98a0-ff1d44c5a15a">RTM_ENTITY_INFO</a>



<a href="https://msdn.microsoft.com/ea72dde4-2d04-4ceb-b718-3ee96bf70464">RtmReleaseEntityInfo</a>
 

 

