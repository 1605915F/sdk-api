---
UID: NF:workspaceruntime.IWorkspaceRegistration2.RemoveResourceEx
title: IWorkspaceRegistration2::RemoveResourceEx
author: windows-sdk-content
description: Notifies the RemoteApp and Desktop Connection runtime that the client is disconnecting the connection.
old-location: termserv\iworkspaceregistration2_removeresourceex.htm
tech.root: TermServ
ms.assetid: dc8b7374-4a64-43a8-947e-0088aa26444e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWorkspaceRegistration2 interface [Remote Desktop Services],RemoveResourceEx method, IWorkspaceRegistration2.RemoveResourceEx, IWorkspaceRegistration2::RemoveResourceEx, RemoveResourceEx, RemoveResourceEx method [Remote Desktop Services], RemoveResourceEx method [Remote Desktop Services],IWorkspaceRegistration2 interface, RemoveResourceEx method [Remote Desktop Services],Workspace object, Workspace object [Remote Desktop Services],RemoveResourceEx method, termserv.iworkspaceregistration2_removeresourceex, workspaceruntime/IWorkspaceRegistration2::RemoveResourceEx
ms.topic: method
req.header: workspaceruntime.h
req.include-header: Workspaceruntime.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1
req.target-min-winversvr: Windows Server 2012 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WorkspaceRuntime.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: WkspRt.exe
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 -
api_name:
 - IWorkspaceRegistration2::RemoveResourceEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWorkspaceRegistration2::RemoveResourceEx


## -description


Not implemented.

Notifies the RemoteApp and Desktop Connection runtime that  the client is disconnecting the connection.


## -parameters




### -param dwCookieConnection [in]

A <b>DWORD</b> value that contains a connection cookie returned by the <a href="https://msdn.microsoft.com/7bb26842-ca30-40e2-b7a2-474dda4ad433">AddResourceEx</a> method.


### -param correlationId [in]

TBD


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/b677863a-c8cc-4ed8-aea4-16de1cba21c4">IWorkspaceRegistration2</a>
 

 

