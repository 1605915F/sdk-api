---
UID: NF:shldisp.IShellFolderViewDual.PopupItemMenu
title: IShellFolderViewDual::PopupItemMenu (shldisp.h)
author: windows-sdk-content
description: Creates a shortcut menu for the specified item and returns the selected command string.
old-location: shell\IShellFolderViewDual_PopupItemMenu.htm
tech.root: shell
ms.assetid: f44e91b7-b651-4b6f-9583-cd9335ae6369
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IShellFolderViewDual interface [Windows Shell],PopupItemMenu method, IShellFolderViewDual.PopupItemMenu, IShellFolderViewDual::PopupItemMenu, PopupItemMenu, PopupItemMenu method [Windows Shell], PopupItemMenu method [Windows Shell],IShellFolderViewDual interface, _shell_IShellFolderViewDual_PopupItemMenu, shell.IShellFolderViewDual_PopupItemMenu, shldisp/IShellFolderViewDual::PopupItemMenu
ms.topic: method
req.header: shldisp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shldisp.idl
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
 - Shldisp.h
api_name:
 - IShellFolderViewDual.PopupItemMenu
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellFolderViewDual::PopupItemMenu


## -description


Creates a shortcut menu for the specified item and returns the selected command string.


## -parameters




### -param pfi [in, optional]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb787810(v=VS.85).aspx">FolderItem</a>*</b>

The FolderItem for which to create a shortcut menu.


### -param vx [in, optional]

Type: <b>VARIANT</b>

Optional.


### -param vy [in, optional]

Type: <b>VARIANT</b>

Optional.


### -param pbs [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms221069(v=VS.85).aspx">BSTR</a>*</b>

The command string.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/48135f9d-ee80-4dec-87dc-83f407c25777">IShellFolderViewDual</a>



<a href="https://msdn.microsoft.com/f53b779e-a015-4b17-b04d-e0739cba8168">IShellFolderViewDual2</a>



<a href="https://msdn.microsoft.com/1aa70db8-4225-49de-8b8f-ec86b1aafa22">IShellFolderViewDual3</a>
 

 

