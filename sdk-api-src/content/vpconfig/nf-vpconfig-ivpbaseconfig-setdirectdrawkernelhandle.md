---
UID: NF:vpconfig.IVPBaseConfig.SetDirectDrawKernelHandle
title: IVPBaseConfig::SetDirectDrawKernelHandle (vpconfig.h)
author: windows-sdk-content
description: The SetDirectDrawKernelHandle method sets the kernel-mode handle to the DirectDraw object. This handle enables the device's mini-driver to communicate with DirectDraw.
old-location: dshow\ivpbaseconfig_setdirectdrawkernelhandle.htm
tech.root: DirectShow
ms.assetid: f3a04341-6cca-4fb4-bf47-30659d039a0d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVPBaseConfig interface [DirectShow],SetDirectDrawKernelHandle method, IVPBaseConfig.SetDirectDrawKernelHandle, IVPBaseConfig::SetDirectDrawKernelHandle, IVPBaseConfigSetDirectDrawKernelHandle, SetDirectDrawKernelHandle, SetDirectDrawKernelHandle method [DirectShow], SetDirectDrawKernelHandle method [DirectShow],IVPBaseConfig interface, dshow.ivpbaseconfig_setdirectdrawkernelhandle, vpconfig/IVPBaseConfig::SetDirectDrawKernelHandle
ms.topic: method
req.header: vpconfig.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Vpconfig.h
api_name:
 - IVPBaseConfig.SetDirectDrawKernelHandle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVPBaseConfig::SetDirectDrawKernelHandle


## -description



The <code>SetDirectDrawKernelHandle</code> method sets the kernel-mode handle to the DirectDraw object. This handle enables the device's mini-driver to communicate with DirectDraw.




## -parameters




### -param dwDDKernelHandle [in]

Specifies the kernel-mode handle of the DirectDraw object.


## -returns



Returns an <b>HRESULT</b> value.




## -remarks



Include Dvp.h and Vptype.h before Vpconfig.h.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd390567(v=VS.85).aspx">IVPBaseConfig Interface</a>
 

 

