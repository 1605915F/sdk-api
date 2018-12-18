---
UID: NF:sensevts.ISensLogon.DisplayLock
title: ISensLogon::DisplayLock
author: windows-sdk-content
description: The DisplayLock method notifies an application that the screen display is locked.
old-location: sens\isenslogon_displaylock.htm
tech.root: Sens
ms.assetid: 1675ffc7-7031-492d-bf39-64281a16a074
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DisplayLock, DisplayLock method [SENS], DisplayLock method [SENS],ISensLogon interface, ISensLogon interface [SENS],DisplayLock method, ISensLogon.DisplayLock, ISensLogon::DisplayLock, _zaw_isenslogon_displaylock, sens.isenslogon_displaylock, sensevts/ISensLogon::DisplayLock, syncmgr.isenslogon_displaylock
ms.topic: method
req.header: sensevts.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: Sensevts.tlb
req.lib: 
req.dll: Sens.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Sens.dll
api_name:
 - ISensLogon.DisplayLock
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISensLogon::DisplayLock


## -description


The 
<b>DisplayLock</b> method notifies an application that the screen display is locked.


## -parameters




### -param bstrUserName [in]

The name of a current user.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method returns successfully.

</td>
</tr>
</table>
 




## -remarks



SENS calls this method to notify an application that the screen display is locked.

<div class="alert"><b>Important</b>  This function will not work with multiple logins through Remote Desktop Services and does not support Remote Desktop Services or Fast-User Switching scenarios. Desktop applications can register for session changes notifications by calling <a href="https://msdn.microsoft.com/5067bb03-d8d5-41ce-b187-04d7dd22a028">WTSRegisterSessionNotification</a>. Services can handle session change notifications via SERVICE_CONTROL_SESSIONCHANGE control codes in their <a href="https://msdn.microsoft.com/bb1b863f-e29f-496f-a50e-9ea524fe8603">HandlerEx</a> callback function.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/f313588f-6257-4a0d-b95a-aabc0bc64b53">About System Event Notification Service</a>



<a href="https://msdn.microsoft.com/en-us/library/ms686510(v=VS.85).aspx">IEventSubscription</a>



<a href="https://msdn.microsoft.com/en-us/library/ms685465(v=VS.85).aspx">IEventSubscription::PutPublisherProperty</a>



<a href="https://msdn.microsoft.com/77c02510-6386-4f6d-af1a-e7337f5d347d">ISensLogon</a>



<a href="https://msdn.microsoft.com/aa1b1beb-f59a-4990-84e1-deca1432f6cf">ISensLogon::DisplayUnLock</a>



<a href="https://msdn.microsoft.com/47531e1f-e2d4-4475-a109-e213c903a7ba">ISensLogon::StartScreenSaver</a>



<a href="https://msdn.microsoft.com/61a6434b-1a80-4a37-9175-636c3792a865">ISensLogon::StopScreenSaver</a>
 

 

