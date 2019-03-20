---
UID: NN:sensorsapi.ISensorEvents
title: ISensorEvents (sensorsapi.h)
author: windows-sdk-content
description: The callback interface you must implement if you want to receive sensor events.
old-location: winsensors\isensorevents.htm
tech.root: SensorsAPI
ms.assetid: 41acbb4f-b4f8-4573-a993-ed93ec9494f0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ISensorEvents, ISensorEvents interface [WinSensors], ISensorEvents interface [WinSensors],described, sensorsapi/ISensorEvents, winsensors.isensorevents
ms.topic: interface
req.header: sensorsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Sensorsapi.lib
req.dll: Sensorsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - sensorsapi.dll
api_name:
 - ISensorEvents
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISensorEvents interface


## -description


The callback interface you must implement if you want to receive sensor events.

To subscribe to events for a particular sensor, call <a href="https://msdn.microsoft.com/8e2f7edc-894f-4258-8948-2a3d4df532c3">ISensor::SetEventSink</a>.

In addition to the methods inherited from <b>IUnknown</b>, the <b>ISensorEvents</b> interface exposes the following methods.


## -see-also




<a href="https://msdn.microsoft.com/872de1e9-20f9-409b-9917-24b13a8cc08a">COM Interfaces</a>
 

 

