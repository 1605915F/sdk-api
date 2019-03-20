---
UID: NF:bdaiface.IBDA_Topology.CreateTopology
title: IBDA_Topology::CreateTopology (bdaiface.h)
author: windows-sdk-content
description: The CreateTopology method associates an instance of an input pin with an instance of an output pin.
old-location: mstv\ibda_topology_createtopology.htm
tech.root: mstv
ms.assetid: 6c91e614-b1b4-4cf5-90d2-15823e5952cb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateTopology, CreateTopology method [Microsoft TV Technologies], CreateTopology method [Microsoft TV Technologies],IBDA_Topology interface, IBDA_Topology interface [Microsoft TV Technologies],CreateTopology method, IBDA_Topology.CreateTopology, IBDA_Topology::CreateTopology, IBDA_TopologyCreateTopology, bdaiface/IBDA_Topology::CreateTopology, mstv.ibda_topology_createtopology
ms.topic: method
req.header: bdaiface.h
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
 - bdaiface.h
api_name:
 - IBDA_Topology.CreateTopology
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBDA_Topology::CreateTopology


## -description



The <b>CreateTopology</b> method associates an instance of an input pin with an instance of an output pin.




## -parameters




### -param ulInputPinId [in]

Specifies the identifier of the input pin for which a topology should be created.


### -param ulOutputPinId [in]

Specifies the identifier of the output pin for which a topology should be created.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd693447(v=VS.85).aspx">IBDA_Topology Interface</a>
 

 

