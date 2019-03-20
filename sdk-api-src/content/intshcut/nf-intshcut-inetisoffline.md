---
UID: NF:intshcut.InetIsOffline
title: InetIsOffline function (intshcut.h)
author: windows-sdk-content
description: Determines whether the system is connected to the Internet.
old-location: shell\InetIsOffline.htm
tech.root: shell
ms.assetid: e0afac1c-c083-4b60-a30f-5dfc1a4b8fd3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InetIsOffline, InetIsOffline function [Windows Shell], _win32_InetIsOffline, intshcut/InetIsOffline, shell.InetIsOffline
ms.topic: function
req.header: intshcut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
req.lib: 
req.dll: Url.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Url.dll
api_name:
 - InetIsOffline
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# InetIsOffline function


## -description


Determines whether the system is connected to the Internet.


## -parameters




### -param dwFlags

Type: <b>DWORD</b>

The input flags for the function. This must be set to zero.


## -returns



Type: <b>BOOL</b>

Returns <b>TRUE</b> if the local system is not currently connected to the Internet. Returns <b>FALSE</b> if the local system is connected to the Internet or if no attempt has yet been made to connect to the Internet.



