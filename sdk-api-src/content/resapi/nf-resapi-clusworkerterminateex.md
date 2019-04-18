---
UID: NF:resapi.ClusWorkerTerminateEx
title: ClusWorkerTerminateEx function (resapi.h)
author: windows-sdk-content
description: Waits for a worker thread to terminate up to the specified timeout.
old-location: mscs\clusworkerterminateex.htm
tech.root: MsCS
ms.assetid: e2dda7c0-01d4-49e5-bc57-3fa07495d536
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ClusWorkerTerminateEx, ClusWorkerTerminateEx function [Failover Cluster], mscs.clusworkerterminateex, resapi/ClusWorkerTerminateEx
ms.topic: function
req.header: resapi.h
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
 - ClusWorkerTerminateEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ClusWorkerTerminateEx function


## -description


Waits for a worker thread to terminate up to the specified timeout.  This function can signal the thread to terminate before wait starts, or just wait passively if specified.


## -parameters




### -param ClusWorker [in, out]

Pointer to a <a href="https://msdn.microsoft.com/559b147f-8e8a-4bc7-94ea-e2042f288b6d">CLUS_WORKER</a> structure describing the 
       worker thread to terminate.


### -param TimeoutInMilliseconds [in]

The timeout in milliseconds.


### -param WaitOnly [in]

If set <b>TRUE</b>, the function will wait for up to specified timeout without signaling the thread to terminate; otherwise it will signal the thread to terminate before waiting for the thread.


## -returns



Returns a system error code on failure.

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
All worker threads are terminated.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WAIT_TIMEOUT</b></dt>
</dl>
</td>
<td width="60%">
The worker thread is not terminated within the specified timeout.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/559b147f-8e8a-4bc7-94ea-e2042f288b6d">CLUS_WORKER</a>



<a href="https://msdn.microsoft.com/e8833961-ac0e-4d8c-a57e-5aabdb2c8c96">ClusWorkerCheckTerminate</a>



<a href="https://msdn.microsoft.com/a7e8f8ad-c9de-4c6b-8926-b9a46d85924d">ClusWorkerCreate</a>



<a href="https://msdn.microsoft.com/d143a860-92fe-4fa9-b0d7-d591376a0209">ClusWorkerTerminate</a>



<a href="https://msdn.microsoft.com/af9bcdcf-ca92-438b-94f2-f0e7529952fb">ClusWorkersTerminate</a>



<a href="https://msdn.microsoft.com/47436aab-a513-423b-8287-e467954e1dc1">Thread Management Utility Functions</a>
 

 

