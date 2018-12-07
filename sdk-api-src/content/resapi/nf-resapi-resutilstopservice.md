---
UID: NF:resapi.ResUtilStopService
title: ResUtilStopService function
author: windows-sdk-content
description: Stops a service identified by a handle. The PRESUTIL_STOP_SERVICE type defines a pointer to this function.
old-location: mscs\resutilstopservice.htm
tech.root: mscs
ms.assetid: 22be9285-7db6-43dc-bf41-08187bbefc41
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PRESUTIL_STOP_SERVICE, PRESUTIL_STOP_SERVICE function [Failover Cluster], ResUtilStopService, ResUtilStopService function [Failover Cluster], _wolf_resutilstopservice, mscs.resutilstopservice, resapi/PRESUTIL_STOP_SERVICE, resapi/ResUtilStopService
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: resapi.h
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
 - ResUtilStopService
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilStopService function


## -description


Stops a <a href="https://msdn.microsoft.com/en-us/library/Aa372937(v=VS.85).aspx">service</a> identified by a handle. The <b>PRESUTIL_STOP_SERVICE</b> type defines a pointer to this function.


## -parameters




### -param hServiceHandle [in]

Handle of the service to stop.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>. The following is a possible error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_TIMEOUT</b></dt>
</dl>
</td>
<td width="60%">
Service did not stop after a reasonable number of retries.

</td>
</tr>
</table>
 




## -remarks



The  <b>ResUtilStopService</b> utility function closes the handle specified in <i>hServiceHandle</i> when it stops the service.



