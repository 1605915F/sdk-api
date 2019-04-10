---
UID: NF:shobjidl_core.IShellLibrary.GetDefaultSaveFolder
title: IShellLibrary::GetDefaultSaveFolder (shobjidl_core.h)
author: windows-sdk-content
description: Retrieves the default target folder that the library uses for save operations.
old-location: shell\IShellLibrary_GetDefaultSaveFolder.htm
tech.root: shell
ms.assetid: 4bc501b1-2fc4-49ce-a16b-e254a3a40f46
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDefaultSaveFolder, GetDefaultSaveFolder method [Windows Shell], GetDefaultSaveFolder method [Windows Shell],IShellLibrary interface, IShellLibrary interface [Windows Shell],GetDefaultSaveFolder method, IShellLibrary.GetDefaultSaveFolder, IShellLibrary::GetDefaultSaveFolder, _shell_IShellLibrary_GetDefaultSaveFolder, shell.IShellLibrary_GetDefaultSaveFolder, shobjidl_core/IShellLibrary::GetDefaultSaveFolder
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - shobjidl_core.h
api_name:
 - IShellLibrary.GetDefaultSaveFolder
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellLibrary::GetDefaultSaveFolder


## -description


Retrieves the default target folder that the library uses  for save operations.


## -parameters




### -param dsft [in]

Type: <b><a href="https://msdn.microsoft.com/51478854-03b2-4e1a-bc07-b9ca7e6cc33d">DEFAULTSAVEFOLDERTYPE</a></b>

The <a href="https://msdn.microsoft.com/51478854-03b2-4e1a-bc07-b9ca7e6cc33d">DEFAULTSAVEFOLDERTYPE</a>  value that specifies the save folder to get.


### -param riid [in]

Type: <b>REFIID</b>

A reference to the IID of the interface to get in <i>ppv</i> that will represent the save location.   This value is typically IID_IShellItem,  but it can also be IID_IShellItem2 or the IID of any other interface that is implemented by CShellItem.


### -param ppv [out]

Type: <b>void**</b>

A  pointer  to the interface requested in <i>riid</i>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



For best results, use the <b>IID_PPV_ARGS</b> macro, defined in Objbase.h,  for  the <i>riid</i> and <i>ppv</i> parameters. This macro provides the correct IID based on the interface pointed to by the value in <i>ppv</i>, which eliminates the possibility of a coding error.




## -see-also




<a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>



<a href="https://msdn.microsoft.com/e54d8385-ec67-4825-ad7c-431807a4fcb4">IShellItem2</a>



<a href="https://msdn.microsoft.com/c1ef3d22-7c88-42b0-93a2-5d1b75c327ba">IShellLibrary</a>



<a href="https://msdn.microsoft.com/12F6E6AE-2776-408c-B9AC-E885BE93C27F">Library Description Schema</a>



<a href="https://msdn.microsoft.com/19DA68B2-FCB6-443d-A3CD-0BF2F429B149">Windows Libraries</a>
 

 

