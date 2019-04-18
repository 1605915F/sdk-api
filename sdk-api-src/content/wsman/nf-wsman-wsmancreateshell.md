---
UID: NF:wsman.WSManCreateShell
title: WSManCreateShell function (wsman.h)
author: windows-sdk-content
description: Creates a shell object.
old-location: winrm\wsmancreateshell.htm
tech.root: winrm
ms.assetid: 901c0a2d-d25f-451c-8d6c-83662f1f1061
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WSManCreateShell, WSManCreateShell function [Windows Remote Management], winrm.wsmancreateshell, wsman/WSManCreateShell
ms.topic: function
req.header: wsman.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
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
 - WSManCreateShell
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Management Framework on Windows Server 2008 with SP2 and Windows Vista with SP2
ms.custom: 19H1
---

# WSManCreateShell function


## -description


Creates a shell object. The returned shell handle identifies an object that defines the context in which commands can be run. The context is defined by the environment variables, the input and output streams, and the working directory. The context can directly affect the behavior of a command. A shell context is created on the remote computer specified by the connection parameter and authenticated by using the credentials parameter.


## -parameters




### -param session [in, out]

Specifies the session handle returned by a <a href="https://msdn.microsoft.com/5123d876-5123-4fa4-8f6f-859a26aad825">WSManCreateSession</a> call. This parameter cannot be <b>NULL</b>.


### -param flags

Reserved for future use. Must be zero.


### -param resourceUri [in]

Defines the shell type to create. The shell type is defined by a unique URI. The actual shell object returned by the call is dependent on the URI specified. This parameter cannot be <b>NULL</b>. To create a Windows cmd.exe shell, use the <b>WSMAN_CMDSHELL_URI</b> resource URI.


### -param startupInfo [in, optional]

A pointer to a <a href="https://msdn.microsoft.com/a9e004de-b157-4ad3-a463-a42ccb56f1ba">WSMAN_SHELL_STARTUP_INFO</a> structure that specifies the input and output streams, working directory, idle time-out, and options for the shell.

If this parameter is <b>NULL</b>, the default values will be used.


### -param options [in, optional]

A pointer to a <a href="https://msdn.microsoft.com/16a1447c-d764-44bf-9c62-064769ead0f3">WSMAN_OPTION_SET</a> structure that specifies a set of options for the shell.


### -param createXml [in, optional]

A pointer to a <a href="https://msdn.microsoft.com/4ff574d4-04b0-47c3-808f-867d6815bffc">WSMAN_DATA</a> structure that defines an open context for the shell. The content should be a valid XML string. This parameter can be <b>NULL</b>.


### -param async [in]

Defines an asynchronous structure. The asynchronous structure contains an optional user context and a mandatory callback function. See the <a href="https://msdn.microsoft.com/9391e1a8-7048-49b8-9dc4-1da25b190238">WSMAN_SHELL_ASYNC</a> structure for more information.  This parameter cannot be <b>NULL</b> and should be closed by calling the <a href="https://msdn.microsoft.com/1da452ef-5842-4d8d-941b-09fa57393ebb">WSManCloseShell</a> method.


### -param shell [out]

Defines a shell handle that uniquely identifies the shell object. The resource handle is used to track the client endpoint for the shell and is used by other WinRM methods to interact with the shell object. The shell object should be deleted by calling the <a href="https://msdn.microsoft.com/1da452ef-5842-4d8d-941b-09fa57393ebb">WSManCloseShell</a> method. This parameter cannot be <b>NULL</b>.


## -returns



This function does not return a value.



