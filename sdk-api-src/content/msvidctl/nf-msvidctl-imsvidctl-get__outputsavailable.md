---
UID: NF:msvidctl.IMSVidCtl.get__OutputsAvailable
title: IMSVidCtl::get__OutputsAvailable (msvidctl.h)
author: windows-sdk-content
description: The get__OutputsAvailable method retrieves the output devices that are available in a specified category.
old-location: mstv\imsvidctl_get__outputsavailable.htm
tech.root: mstv
ms.assetid: 8242712a-9112-456b-b76d-1f382c9b637f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidCtl interface [Microsoft TV Technologies],get__OutputsAvailable method, IMSVidCtl.get__OutputsAvailable, IMSVidCtl::get__OutputsAvailable, IMSVidCtlget__OutputsAvailable, get__OutputsAvailable, get__OutputsAvailable method [Microsoft TV Technologies], get__OutputsAvailable method [Microsoft TV Technologies],IMSVidCtl interface, mstv.imsvidctl_get__outputsavailable, msvidctl/IMSVidCtl::get__OutputsAvailable
ms.topic: method
req.header: msvidctl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Msvidctl.idl
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
 - msvidctl.h
api_name:
 - IMSVidCtl.get__OutputsAvailable
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidCtl::get__OutputsAvailable


## -description


The <b>get__OutputsAvailable</b> method retrieves the output devices that are available in a specified category.

This method is currently not supported.


## -parameters




### -param CategoryGuid [in]

Pointer to a GUID that specifies the category to enumerate.


### -param pVal [out]

Receives an <a href="https://msdn.microsoft.com/54776225-ad60-450b-99b4-851cae60ffa7">IMSVidOutputDevices</a> interface pointer. The caller must release the interface.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -remarks



To obtain the available renderers, use the <a href="https://msdn.microsoft.com/6ab81536-2701-408e-be3a-f44375ef8193">get_AudioRenderersAvailable</a> and <a href="https://msdn.microsoft.com/20e5b2f3-33ea-4b0d-84b8-e4b0b61e0348">get_VideoRenderersAvailable</a> methods.




## -see-also




<a href="https://msdn.microsoft.com/e3ea10ea-bfb4-4c35-9933-5ad0367fd9ee">IMSVidCtl Interface</a>
 

 

