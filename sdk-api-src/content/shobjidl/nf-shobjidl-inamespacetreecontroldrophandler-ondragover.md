---
UID: NF:shobjidl.INameSpaceTreeControlDropHandler.OnDragOver
title: INameSpaceTreeControlDropHandler::OnDragOver
author: windows-sdk-content
description: Called on drag over to set drag effect, as specified.
old-location: shell\INameSpaceTreeControlDropHandler_OnDragOver.htm
tech.root: shell
ms.assetid: 9875bd38-9f1d-479f-bd8a-8deb07aa9b53
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: INameSpaceTreeControlDropHandler interface [Windows Shell],OnDragOver method, INameSpaceTreeControlDropHandler.OnDragOver, INameSpaceTreeControlDropHandler::OnDragOver, OnDragOver, OnDragOver method [Windows Shell], OnDragOver method [Windows Shell],INameSpaceTreeControlDropHandler interface, _shell_INameSpaceTreeControlDropHandler_OnDragOver, shell.INameSpaceTreeControlDropHandler_OnDragOver, shobjidl/INameSpaceTreeControlDropHandler::OnDragOver
ms.topic: method
req.header: shobjidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
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
 - COM
api_location:
 - Shobjidl.h
api_name:
 - INameSpaceTreeControlDropHandler.OnDragOver
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# INameSpaceTreeControlDropHandler::OnDragOver


## -description


Called on drag over to set drag effect, as specified.


## -parameters




### -param psiOver [in]

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> interface representing the item underneath the mouse cursor. Optional.


### -param psiaData [in]

Type: <b><a href="https://msdn.microsoft.com/348213d1-c03f-4c38-9d13-3b1009d94e07">IShellItemArray</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> array containing the items being dragged.


### -param grfKeyState [in]

Type: <b>DWORD</b>

The current state of keyboard modifier keys.


### -param pdwEffect [in, out]

Type: <b>DWORD*</b>

On success, contains a pointer to the drag effect value.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Failing this method blocks the drag operation in the namespace tree control (NSTC).




## -see-also




<a href="https://msdn.microsoft.com/31bb71dd-eed7-48f9-9f6c-f5d7f9d4118e">IDropTarget::DragOver</a>



<a href="https://msdn.microsoft.com/5d2c1783-daeb-488d-93b9-34df2712d849">INameSpaceTreeControlDropHandler</a>
 

 

