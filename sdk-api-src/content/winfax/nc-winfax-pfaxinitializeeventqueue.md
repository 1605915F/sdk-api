---
UID: NC:winfax.PFAXINITIALIZEEVENTQUEUE
title: PFAXINITIALIZEEVENTQUEUE (winfax.h)
author: windows-sdk-content
description: The FaxInitializeEventQueue function creates a fax event queue for the calling fax client application. The queue enables the application to receive notifications of asynchronous events from the fax server.
old-location: fax\_mfax_faxinitializeeventqueue.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_2ip1.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FaxInitializeEventQueueA, FaxInitializeEventQueueW, PFAXINITIALIZEEVENTQUEUE, PFAXINITIALIZEEVENTQUEUE callback, PFAXINITIALIZEEVENTQUEUE callback function [Fax Service], _mfax_faxinitializeeventqueue, fax._mfax_faxinitializeeventqueue, winfax/FaxInitializeEventQueueA, winfax/FaxInitializeEventQueueW, winfax/PFAXINITIALIZEEVENTQUEUE
ms.topic: callback
req.header: winfax.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: FaxInitializeEventQueueW (Unicode) and FaxInitializeEventQueueA (ANSI)
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
 - UserDefined
api_location:
 - Winfax.h
api_name:
 - PFAXINITIALIZEEVENTQUEUE
 - FaxInitializeEventQueueA
 - FaxInitializeEventQueueW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFAXINITIALIZEEVENTQUEUE callback function


## -description


The <b>FaxInitializeEventQueue</b> function creates a fax event queue for the calling fax client application. The queue enables the application to receive notifications of asynchronous events from the fax server.


## -parameters




### -param FaxHandle [in]

Type: <b>HANDLE</b>

Specifies a fax server handle returned by a call to the <a href="https://msdn.microsoft.com/en-us/library/ms691482(v=VS.85).aspx">FaxConnectFaxServer</a> function.


### -param CompletionPort [in]

Type: <b>HANDLE</b>

Specifies a valid handle to an I/O completion port returned by a call to the <a href="https://msdn.microsoft.com/40cb47fc-7b15-47f6-bee2-2611d4686053">CreateIoCompletionPort</a> function. This parameter is required for notification using I/O completion packets. This parameter must be <b>NULL</b> if you specify notification messages. 

                    

For information about I/O completion ports, see <a href="https://msdn.microsoft.com/213c48e8-bb21-43ed-9c00-2a5cf8ac25f0">I/O Completion Ports</a>.


### -param CompletionKey [in]

Type: <b>ULONG_PTR</b>

Specifies a variable that contains a completion key value the fax server includes in each I/O completion packet. This parameter is required for notification using I/O completion packets. This parameter must be <b>NULL</b> if you specify notification messages. For more information, see the following Remarks section.


### -param hWnd [in]

Type: <b>HWND</b>

Handle to a window of the fax client application to notify when an asynchronous event occurs. This parameter is required for notification messages. This parameter must be <b>NULL</b> if you specify notification using I/O completion packets.


### -param MessageStart [in]

Type: <b>UINT</b>

Specifies an unsigned integer that identifies the application's base window message. The application can use this number to determine whether to process the message as a fax server event. For more information, see the <a href="https://msdn.microsoft.com/en-us/library/ms692820(v=VS.85).aspx">FAX_EVENT</a> topic. 

                    

This parameter is required for notification messages. This parameter must be equal to zero if you specify notification using I/O completion packets.


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. GetLastError can return one of the following errors.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
Both the <i>hWnd</i> and <i>CompletionPort</i> parameters are <b>NULL</b>, or both parameters are specified.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>FaxHandle</i> parameter is <b>NULL</b>; or the <i>hWnd</i> parameter is specified but the <i>FaxHandle</i> parameter does not specify a connection with a local fax server; or the <i>MessageStart</i> parameter specifies a message in the range below <a href="https://msdn.microsoft.com/en-us/library/ms644931(v=VS.85).aspx">WM_USER</a>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_DATA</b></dt>
</dl>
</td>
<td width="60%">
The application called the <a href="https://msdn.microsoft.com/en-us/library/ms691325(v=VS.85).aspx">FaxInitializeEventQueue</a> function more than once during a fax service session in Windows 2000. More than one call is supported in Windows XP and Windows Server 2003.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
An error occurred during memory allocation.

</td>
</tr>
</table>
 




## -remarks



An application can specify how the fax server should inform the client application of events. The application can request that the fax server queue I/O completion packets to an I/O completion port, or it can specify notification messages.

A fax client application must call the <b>FaxInitializeEventQueue</b> function before calling <a href="https://msdn.microsoft.com/8121a38b-0fe1-43b8-aed6-4b85af1feba9">GetQueuedCompletionStatus</a> to retrieve the value to specify in the <i>CompletionKey</i> parameter. This value is useful to a message loop that retrieves I/O completion packets from multiple I/O completion ports, using calls to the <a href="https://msdn.microsoft.com/51afb13c-ea7a-407a-9f21-345d84f3b96b">WaitForMultipleObjects</a> function. If you specify a different completion key for each I/O completion port, you can identify the completion port associated with the completion packet.

An application can call the <a href="https://msdn.microsoft.com/8121a38b-0fe1-43b8-aed6-4b85af1feba9">GetQueuedCompletionStatus</a> function to retrieve the queued I/O completion packet for a completed I/O operation. A call to GetQueuedCompletionStatus also returns a pointer to a variable that the function sets to the address of a <a href="https://msdn.microsoft.com/en-us/library/ms692820(v=VS.85).aspx">FAX_EVENT</a> structure. The structure is associated with the I/O completion packet of interest. Call the <a href="https://msdn.microsoft.com/a0393983-cb43-4dfa-91a6-d82a5fb8de12">LocalFree</a> function to free the memory allocated for the <b>FAX_EVENT</b> structure.

After a fax client application receives the <b>FEI_FAXSVC_ENDED</b> message, it will no longer receive fax events from the fax service. To resume receiving fax events, the application must call the <b>FaxInitializeEventQueue</b> function again when the fax service restarts. The application can determine if the fax service is running by using the service control manager. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms691909(v=VS.85).aspx">FaxClose</a> and <a href="https://msdn.microsoft.com/en-us/library/ms692290(v=VS.85).aspx">Enabling an Application to Receive Notifications of Fax Events</a>.

For a list of the asynchronous events that can occur within the fax server, see the <a href="https://msdn.microsoft.com/en-us/library/ms692820(v=VS.85).aspx">FAX_EVENT</a> topic.




## -see-also




<a href="https://msdn.microsoft.com/40cb47fc-7b15-47f6-bee2-2611d4686053">CreateIoCompletionPort</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692820(v=VS.85).aspx">FAX_EVENT</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691947(v=VS.85).aspx">Fax Service Client API Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691909(v=VS.85).aspx">FaxClose</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691482(v=VS.85).aspx">FaxConnectFaxServer</a>



<a href="https://msdn.microsoft.com/en-us/library/ms690875(v=VS.85).aspx">FaxOpenPort</a>



<a href="https://msdn.microsoft.com/8121a38b-0fe1-43b8-aed6-4b85af1feba9">GetQueuedCompletionStatus</a>



<a href="https://msdn.microsoft.com/a0393983-cb43-4dfa-91a6-d82a5fb8de12">LocalFree</a>



<a href="https://msdn.microsoft.com/51afb13c-ea7a-407a-9f21-345d84f3b96b">WaitForMultipleObjects</a>
 

 

