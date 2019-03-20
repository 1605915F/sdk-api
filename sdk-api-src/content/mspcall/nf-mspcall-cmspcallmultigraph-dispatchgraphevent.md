---
UID: NF:mspcall.CMSPCallMultiGraph.DispatchGraphEvent
title: CMSPCallMultiGraph::DispatchGraphEvent (mspcall.h)
author: windows-sdk-content
description: The DispatchGraphEvent method is a static method posted to the RegisterWaitForSingleObject function during initialization.
old-location: tapi3\cmspcallmultigraph_dispatchgraphevent.htm
tech.root: Tapi
ms.assetid: 3f6f9145-1968-4067-936e-918f43ccbbcc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CMSPCallMultiGraph interface [TAPI 2.2],DispatchGraphEvent method, CMSPCallMultiGraph.DispatchGraphEvent, CMSPCallMultiGraph::DispatchGraphEvent, DispatchGraphEvent, DispatchGraphEvent method [TAPI 2.2], DispatchGraphEvent method [TAPI 2.2],CMSPCallMultiGraph interface, _tapi3_cmspcallmultigraph_dispatchgraphevent, mspcall/CMSPCallMultiGraph::DispatchGraphEvent, tapi3.cmspcallmultigraph_dispatchgraphevent
ms.topic: method
req.header: mspcall.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - Mspcall.h
api_name:
 - CMSPCallMultiGraph.DispatchGraphEvent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CMSPCallMultiGraph::DispatchGraphEvent


## -description


The 
<b>DispatchGraphEvent</b> method is a static method posted to the 
<a href="https://msdn.microsoft.com/d0cd8b28-6e20-449a-94dd-cca2be46b812">RegisterWaitForSingleObject</a> function during initialization. This function is called when the filter graph signals the event. The <i>pContext</i> parameter is a pointer to the 
<a href="https://msdn.microsoft.com/6a7fe6ea-8e25-469a-8505-55d48a661cd8">MSPSTREAMCONTEXT</a> structure. The pointers in the structure carry ref counts. The implementation of this method simply casts the <i>pContext</i> argument to type MSPSTREAMCONTEXT *, and then calls 
<a href="https://msdn.microsoft.com/en-us/library/ms726569(v=VS.85).aspx">HandleGraphEvent</a> on the MSP call object whose pointer appears in the structure.


## -parameters




### -param pContext

Contains pointer to 
<a href="https://msdn.microsoft.com/6a7fe6ea-8e25-469a-8505-55d48a661cd8">MSPSTREAMCONTEXT</a> structure.


### -param bFlag

Not used. Required for 
<a href="https://msdn.microsoft.com/d0cd8b28-6e20-449a-94dd-cca2be46b812">RegisterWaitForSingleObject</a>. Set <b>TRUE</b> if wait times out, but time-out in 
<a href="https://msdn.microsoft.com/en-us/library/ms726610(v=VS.85).aspx">CMSPCallMultiGraph::RegisterWaitEvent</a> is set to INFINITE.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms726558(v=VS.85).aspx">CMSPCallMultiGraph</a>
 

 

