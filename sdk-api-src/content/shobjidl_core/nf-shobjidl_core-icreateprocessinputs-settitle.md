---
UID: NF:shobjidl_core.ICreateProcessInputs.SetTitle
title: ICreateProcessInputs::SetTitle (shobjidl_core.h)
author: windows-sdk-content
description: Sets the title that will be passed CreateProcess.
old-location: shell\icreateprocessinputs_settitle.htm
tech.root: shell
ms.assetid: BFCDC5B1-740E-4CE9-8E06-75F3ECA7B7E6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICreateProcessInputs interface [Windows Shell],SetTitle method, ICreateProcessInputs.SetTitle, ICreateProcessInputs::SetTitle, SetTitle, SetTitle method [Windows Shell], SetTitle method [Windows Shell],ICreateProcessInputs interface, shell.icreateprocessinputs_settitle, shobjidl_core/ICreateProcessInputs::SetTitle
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
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
 - shobjidl_core.h
api_name:
 - ICreateProcessInputs.SetTitle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ICreateProcessInputs::SetTitle


## -description


 Sets the title that will be passed <a href="https://msdn.microsoft.com/3ef0a5b2-4d71-4c17-8188-76a4025287fc">CreateProcess</a>.


## -parameters




### -param pszTitle [in]

 A null-terminated string specifying the title that will be passed in the <b>lpTitle</b> member of the <a href="https://msdn.microsoft.com/cf4b795c-52c1-4573-8328-99ee13f68bb3">STARTUPINFO</a> structure passed to <a href="https://msdn.microsoft.com/3ef0a5b2-4d71-4c17-8188-76a4025287fc">CreateProcess</a>. This parameter may not be <b>NULL</b>.


## -returns



<b> S_OK</b> if the method succeeds. Otherwise, an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/3ef0a5b2-4d71-4c17-8188-76a4025287fc">CreateProcess</a>



<a href="https://msdn.microsoft.com/2C1756A3-FF40-4FBF-860D-06BB415DB695">ICreateProcessInputs</a>



<a href="https://msdn.microsoft.com/5A13ABDB-8453-41BE-AF0C-B5A07486CBE6">ICreatingProcess::OnCreating</a>
 

 

