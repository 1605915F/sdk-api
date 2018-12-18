---
UID: NF:shldisp.IShellFolderViewDual.SelectItem
title: IShellFolderViewDual::SelectItem
author: windows-sdk-content
description: Sets the selection state of an item in the view.
old-location: shell\IShellFolderViewDual_SelectItem.htm
tech.root: shell
ms.assetid: fb9bc12f-bf5f-42f2-a1cd-160298f7c73a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IShellFolderViewDual interface [Windows Shell],SelectItem method, IShellFolderViewDual.SelectItem, IShellFolderViewDual::SelectItem, SelectItem, SelectItem method [Windows Shell], SelectItem method [Windows Shell],IShellFolderViewDual interface, _shell_IShellFolderViewDual_SelectItem, shell.IShellFolderViewDual_SelectItem, shldisp/IShellFolderViewDual::SelectItem
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
 - IShellFolderViewDual.SelectItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellFolderViewDual::SelectItem


## -description


Sets the selection state of an item in the view.


## -parameters




### -param pvfi [in]

Type: <b>VARIANT*</b>

A VARIANT object.


### -param dwFlags [in]

Type: <b>int</b>

The flags representing the state of the object.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/48135f9d-ee80-4dec-87dc-83f407c25777">IShellFolderViewDual</a>



<a href="https://msdn.microsoft.com/f53b779e-a015-4b17-b04d-e0739cba8168">IShellFolderViewDual2</a>



<a href="https://msdn.microsoft.com/1aa70db8-4225-49de-8b8f-ec86b1aafa22">IShellFolderViewDual3</a>
 

 

