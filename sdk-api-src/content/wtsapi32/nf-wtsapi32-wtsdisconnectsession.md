---
UID: NF:wtsapi32.WTSDisconnectSession
title: WTSDisconnectSession function
author: windows-sdk-content
description: Disconnects the logged-on user from the specified Remote Desktop Services session without closing the session.
old-location: termserv\wtsdisconnectsession.htm
tech.root: termserv
ms.assetid: 1e9487c2-7678-4f9c-9b0b-e6769718d027
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WTSDisconnectSession, WTSDisconnectSession function [Remote Desktop Services], _win32_wtsdisconnectsession, termserv.wtsdisconnectsession, wtsapi32/WTSDisconnectSession
ms.topic: function
req.header: wtsapi32.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wtsapi32.lib
req.dll: Wtsapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Wtsapi32.dll
 - Ext-MS-Win-Session-WtsApi32-l1-1-0.dll
api_name:
 - WTSDisconnectSession
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WTSDisconnectSession function


## -description


Disconnects the logged-on user from the specified Remote Desktop Services session without closing the session. If the user subsequently logs on to the same Remote Desktop Session Host (RD Session Host) server, the user is reconnected to the same session.


## -parameters




### -param hServer [in]

A handle to an RD Session Host server. Specify a handle opened by the 
<a href="https://msdn.microsoft.com/f0b7dce7-59eb-41b8-9a61-65a69d1cc1f3">WTSOpenServer</a> or <a href="https://msdn.microsoft.com/8122de66-c096-4bd8-95ff-ed64b88afcae">WTSOpenServerEx</a> function, or specify <b>WTS_CURRENT_SERVER_HANDLE</b> to indicate the RD Session Host server on which your application is running.


### -param SessionId [in]

A Remote Desktop Services session identifier. To indicate the current session, specify <b>WTS_CURRENT_SESSION</b>. To retrieve the identifiers of all sessions on a specified RD Session Host server, use the 
<a href="https://msdn.microsoft.com/6f9dd7d4-48dc-411c-85f1-cd1239d1e106">WTSEnumerateSessions</a> function.

To be able to disconnect another user's session, you need to have the Disconnect permission. For more information, see 
<a href="https://msdn.microsoft.com/448a7f9b-bf12-48eb-a3e7-4512ec288d95">Remote Desktop Services Permissions</a>. To modify permissions on a session, use the Remote Desktop Services Configuration administrative tool.

To disconnect sessions running on a virtual machine hosted on a RD Virtualization Host server, you must be a member of the Administrators group on the RD Virtualization Host server.


### -param bWait [in]

Indicates whether the operation is synchronous. Specify <b>TRUE</b> to wait for the operation to complete, or <b>FALSE</b> to return immediately.


## -returns



If the function succeeds, the return value is a nonzero value.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -see-also




<a href="https://msdn.microsoft.com/6f9dd7d4-48dc-411c-85f1-cd1239d1e106">WTSEnumerateSessions</a>
 

 

