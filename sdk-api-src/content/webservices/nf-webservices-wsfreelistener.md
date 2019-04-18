---
UID: NF:webservices.WsFreeListener
title: WsFreeListener function (webservices.h)
author: windows-sdk-content
description: Releases the memory resource associated with a Listener object.
old-location: wsw\wsfreelistener.htm
tech.root: wsw
ms.assetid: 3a8a4cd3-d98e-467b-bbed-5cbd66f892ed
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WsFreeListener, WsFreeListener function [Web Services for Windows], webservices/WsFreeListener, wsw.wsfreelistener
ms.topic: function
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WebServices.lib
req.dll: WebServices.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - WebServices.dll
api_name:
 - WsFreeListener
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# WsFreeListener function


## -description


Releases the memory resource associated with a Listener object.
            The Listener state represented in <a href="https://msdn.microsoft.com/275d0d36-f9a1-49a7-af74-e8967dff574a">WS_LISTENER_STATE</a> must be set to either <b>WS_LISTENER_STATE_CREATED</b> 
                or <b>WS_LISTENER_STATE_CLOSED</b> to be released.
            If a Listener has been successfully opened, then it must be closed 
                using <a href="https://msdn.microsoft.com/6023595a-ac52-4619-a824-df49da887fc5">WsCloseListener</a> before it is released.


## -parameters




### -param listener [in]

A pointer to the <b>Listener</b> object to release.  The pointer must reference a valid <a href="https://msdn.microsoft.com/2e771c56-4a07-4c8e-92c1-ffcbf74cd1aa">WS_LISTENER</a> returned
                    by <a href="https://msdn.microsoft.com/2e592fd2-cf88-4f87-a71b-1c3416917fa7">WsCreateListener</a>.  The referenced value may not be <b>NULL</b>.
                


## -returns



This function does not return a value.



