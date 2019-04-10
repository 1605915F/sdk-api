---
UID: NF:wtsapi32.WTSCreateListenerA
title: WTSCreateListenerA function (wtsapi32.h)
author: windows-sdk-content
description: Creates a new Remote Desktop Services listener or configures an existing listener.
old-location: termserv\wtscreatelistener.htm
tech.root: TermServ
ms.assetid: 057facde-43b6-44c4-944a-7ad7854ec1e6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WTSCreateListener, WTSCreateListener function [Remote Desktop Services], WTSCreateListenerA, WTSCreateListenerW, WTS_LISTENER_CREATE, WTS_LISTENER_UPDATE, termserv.wtscreatelistener, wtsapi32/WTSCreateListener, wtsapi32/WTSCreateListenerA, wtsapi32/WTSCreateListenerW
ms.topic: function
req.header: wtsapi32.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: WTSCreateListenerW (Unicode) and WTSCreateListenerA (ANSI)
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
api_name:
 - WTSCreateListener
 - WTSCreateListenerA
 - WTSCreateListenerW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WTSCreateListenerA function


## -description


Creates a new Remote Desktop Services listener or configures an existing listener.


## -parameters




### -param hServer [in]

A handle to an RD Session Host server. Always set this  parameter to <b>WTS_CURRENT_SERVER_HANDLE</b>.


### -param pReserved [in]

This parameter is reserved. Always set this parameter to <b>NULL</b>.


### -param Reserved [in]

This parameter is reserved. Always set this parameter to zero.


### -param pListenerName [in]

A pointer to a null-terminated string that contains the name of the listener to create or configure.


### -param pBuffer [in]

A pointer to a <a href="https://msdn.microsoft.com/051cab0b-701c-4bb9-8728-6b383cdb8e6a">WTSLISTENERCONFIG</a> structure that contains configuration information for the listener.


### -param flag [in]

The purpose of the call. This parameter can be one of the following values.



#### WTS_LISTENER_CREATE (1 (0x1))

Create a new listener.



#### WTS_LISTENER_UPDATE (16 (0x10))

Update the settings of an existing listener.


## -returns



If the function succeeds, the return value is a nonzero value.

If the function fails, the return value is zero. To get extended error information, call 
the <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function.




## -remarks



This function creates or configures a listener that uses   <a href="https://msdn.microsoft.com/442c3c7f-d04b-4dcd-945d-f6e0168c59d5">Remote Desktop Protocol</a> (RDP). Always set the <b>version</b> member of the <a href="https://msdn.microsoft.com/051cab0b-701c-4bb9-8728-6b383cdb8e6a">WTSLISTENERCONFIG</a> structure that is pointed to by the <i>pBuffer</i> parameter to one.

This function does not create or configure the security descriptor of the listener. When you call this function to create a new listener, the function assigns the default security descriptor to the new listener. To modify the security descriptor, call the <a href="https://msdn.microsoft.com/bc90d526-e252-4506-b781-66da5bd66ced">WTSSetListenerSecurity</a> function. For more information about security descriptors, see  <a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">SECURITY_DESCRIPTOR</a>.

This function does not validate the settings for the new listener. Be sure that the settings are valid before calling this function.




## -see-also




<a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">SECURITY_DESCRIPTOR</a>



<a href="https://msdn.microsoft.com/e3e8b35d-9d18-4611-a898-72ca13e40d33">SECURITY_INFORMATION</a>



<a href="https://msdn.microsoft.com/051cab0b-701c-4bb9-8728-6b383cdb8e6a">WTSLISTENERCONFIG</a>



<a href="https://msdn.microsoft.com/bc90d526-e252-4506-b781-66da5bd66ced">WTSSetListenerSecurity</a>
 

 

