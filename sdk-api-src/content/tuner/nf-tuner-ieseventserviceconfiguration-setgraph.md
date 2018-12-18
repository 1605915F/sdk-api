---
UID: NF:tuner.IESEventServiceConfiguration.SetGraph
title: IESEventServiceConfiguration::SetGraph
author: windows-sdk-content
description: Attaches an event service that implements the IESEventService interface to a filter graph. This method allows the processing of events that support the IESEvent interface from devices in the graph.
old-location: mstv\ieseventserviceconfiguration_setgraph.htm
tech.root: mstv
ms.assetid: 0aee92b4-740a-4c5a-a64e-9de08d1c35c2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IESEventServiceConfiguration interface [Microsoft TV Technologies],SetGraph method, IESEventServiceConfiguration.SetGraph, IESEventServiceConfiguration::SetGraph, SetGraph, SetGraph method [Microsoft TV Technologies], SetGraph method [Microsoft TV Technologies],IESEventServiceConfiguration interface, mstv.ieseventserviceconfiguration_setgraph, tuner/IESEventServiceConfiguration::SetGraph
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
 - tuner.h
api_name:
 - IESEventServiceConfiguration.SetGraph
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IESEventServiceConfiguration::SetGraph


## -description


Attaches an event service that implements the <a href="https://msdn.microsoft.com/2720d616-18a6-488e-98ef-565768c22c2a">IESEventService</a>  interface to a filter  graph. This method allows the processing of events that support the <a href="https://msdn.microsoft.com/3c375480-c6df-4bb0-b417-5765b0bed9bf">IESEvent</a> interface from devices in the graph. 


## -parameters




### -param pGraph [in]

Pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd389989(v=VS.85).aspx">IFilterGraph</a> interface that is attached to the <a href="https://msdn.microsoft.com/2720d616-18a6-488e-98ef-565768c22c2a">IESEventService</a> event service.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/2720d616-18a6-488e-98ef-565768c22c2a">IESEventService</a>



<a href="https://msdn.microsoft.com/0b901732-42e1-4f50-904c-75d8202bb5b7">IESEventServiceConfiguration</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd389989(v=VS.85).aspx">IFilterGraph</a>
 

 

