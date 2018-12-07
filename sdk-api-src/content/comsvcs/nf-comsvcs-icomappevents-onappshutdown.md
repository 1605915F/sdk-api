---
UID: NF:comsvcs.IComAppEvents.OnAppShutdown
title: IComAppEvents::OnAppShutdown
author: windows-sdk-content
description: Generated when an application server shuts down.
old-location: cos\icomappevents_onappshutdown.htm
tech.root: cossdk
ms.assetid: d4e35147-48c4-4c77-a648-ffd317aa7861
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComAppEvents interface [COM+],OnAppShutdown method, IComAppEvents.OnAppShutdown, IComAppEvents::OnAppShutdown, OnAppShutdown, OnAppShutdown method [COM+], OnAppShutdown method [COM+],IComAppEvents interface, _dtc_IComAppEvents_OnAppShutdown, comsvcs/IComAppEvents::OnAppShutdown, cos.icomappevents_onappshutdown
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
 - IComAppEvents.OnAppShutdown
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComAppEvents::OnAppShutdown


## -description


Generated when an application server shuts down.


## -parameters




### -param pInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/f4aa0892-4c93-42ea-adc6-1b304b917389">COMSVCSEVENTINFO</a> structure.


### -param guidApp [in]

The globally unique identifier (GUID) of the application.


## -returns



The user verifies the return values from this method.




## -see-also




<a href="https://msdn.microsoft.com/61ae1926-601b-4d97-80e4-d2d2098ced39">IComAppEvents</a>
 

 

