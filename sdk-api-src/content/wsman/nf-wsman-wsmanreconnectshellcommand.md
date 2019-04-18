---
UID: NF:wsman.WSManReconnectShellCommand
title: WSManReconnectShellCommand function (wsman.h)
author: windows-sdk-content
description: Reconnects a previously disconnected command.
old-location: winrm\wsmanreconnectshellcommand.htm
tech.root: winrm
ms.assetid: 3894BB74-4EAA-46D3-ACB2-AFDD3517A9C1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WSManReconnectShellCommand, WSManReconnectShellCommand function [Windows Remote Management], winrm.wsmanreconnectshellcommand, wsman/WSManReconnectShellCommand
ms.topic: function
req.header: wsman.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WsmSvc.lib
req.dll: WsmSvc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - WsmSvc.dll
api_name:
 - WSManReconnectShellCommand
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# WSManReconnectShellCommand function


## -description


Reconnects a previously disconnected command.


## -parameters




### -param commandHandle [in, out]

Specifies the handle returned by a <a href="https://msdn.microsoft.com/8f5c89f8-418c-4a4d-9a52-0fc01ec636b2">WSManRunShellCommand</a> call or a <a href="https://msdn.microsoft.com/860EC6F8-35A9-4C12-9247-4E14E6B1D66A">WSManConnectShellCommand</a> call. This parameter cannot be NULL.


### -param flags

Reserved for future use. Must be set to zero.


### -param async [in]

Defines an asynchronous structure which will contain an optional user context and a mandatory callback function. See the <a href="https://msdn.microsoft.com/9391e1a8-7048-49b8-9dc4-1da25b190238">WSMAN_SHELL_ASYNC</a> structure for more information. This parameter cannot be NULL.


## -returns



This function does not return a value.



