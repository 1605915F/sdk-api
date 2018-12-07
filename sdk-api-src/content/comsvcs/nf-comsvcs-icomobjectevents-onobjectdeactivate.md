---
UID: NF:comsvcs.IComObjectEvents.OnObjectDeactivate
title: IComObjectEvents::OnObjectDeactivate
author: windows-sdk-content
description: Generated when the JIT-activated object is freed by SetComplete or SetAbort.
old-location: cos\icomobjectevents_onobjectdeactivate.htm
tech.root: cossdk
ms.assetid: 3284da44-bcc4-49eb-9aa8-40061bf51869
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComObjectEvents interface [COM+],OnObjectDeactivate method, IComObjectEvents.OnObjectDeactivate, IComObjectEvents::OnObjectDeactivate, OnObjectDeactivate, OnObjectDeactivate method [COM+], OnObjectDeactivate method [COM+],IComObjectEvents interface, _dtc_IComObjectEvents_OnObjectDeactivate, comsvcs/IComObjectEvents::OnObjectDeactivate, cos.icomobjectevents_onobjectdeactivate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: comsvcs.h
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
 - ComSvcs.h
api_name:
 - IComObjectEvents.OnObjectDeactivate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComObjectEvents::OnObjectDeactivate


## -description


Generated when the JIT-activated object is freed by <a href="https://msdn.microsoft.com/8ff25b68-fcb3-4e11-9c74-b49b31806796">SetComplete</a> or <a href="https://msdn.microsoft.com/c254305f-1fc5-417e-b93b-d5e2b36e9e39">SetAbort</a>.


## -parameters




### -param pInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/f4aa0892-4c93-42ea-adc6-1b304b917389">COMSVCSEVENTINFO</a> structure.


### -param CtxtID [in]

The GUID of the current context.


### -param ObjectID [in]

The JIT-activated object.


## -returns



The user verifies the return values from this method.




## -see-also




<a href="https://msdn.microsoft.com/4354fc5b-4d72-4a56-b246-2ae2cf9b5ae1">IComObjectEvents</a>
 

 

