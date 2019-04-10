---
UID: NF:msajtransport.AllJoynEventSelect
title: AllJoynEventSelect function (msajtransport.h)
author: windows-sdk-content
description: Provides AllJoyn transport functionality similar to the TCP socket WSAEventSelect functionality.
old-location: alljoyn\alljoyneventselect.htm
tech.root: AllJoyn
ms.assetid: 8E3A3631-50D5-4947-9C0E-672C08D7292A
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: AllJoynEventSelect, AllJoynEventSelect function [AllJoyn API], alljoyn.alljoyneventselect, msajtransport/AllJoynEventSelect
ms.topic: function
req.header: msajtransport.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2016 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: MSAJApi.lib
req.dll: MSAJApi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - MSAJApi.dll
api_name:
 - AllJoynEventSelect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# AllJoynEventSelect function


## -description


Provides AllJoyn transport functionality similar to the TCP socket <a href="https://msdn.microsoft.com/f98a71e4-47fb-47a4-b37e-e4cc801a8f98">WSAEventSelect</a>  functionality.


## -parameters




### -param connectedBusHandle [in]

Pipe handle.


### -param eventHandle [in]

Handle to the event to be set when any of the events in bit mask happens.


### -param eventTypes [in]

Bit mask of events to select.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.



