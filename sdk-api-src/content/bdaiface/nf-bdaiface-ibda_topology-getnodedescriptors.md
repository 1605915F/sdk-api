---
UID: NF:bdaiface.IBDA_Topology.GetNodeDescriptors
title: IBDA_Topology::GetNodeDescriptors (bdaiface.h)
author: windows-sdk-content
description: The GetNodeDescriptors method retrieves a list of descriptors for the nodes in the topology.
old-location: mstv\ibda_topology_getnodedescriptors.htm
tech.root: mstv
ms.assetid: 4bbfa1d1-7101-4ca6-b6dc-e66b3c49857d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetNodeDescriptors, GetNodeDescriptors method [Microsoft TV Technologies], GetNodeDescriptors method [Microsoft TV Technologies],IBDA_Topology interface, IBDA_Topology interface [Microsoft TV Technologies],GetNodeDescriptors method, IBDA_Topology.GetNodeDescriptors, IBDA_Topology::GetNodeDescriptors, IBDA_TopologyGetNodeDescriptors, bdaiface/IBDA_Topology::GetNodeDescriptors, mstv.ibda_topology_getnodedescriptors
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
 - Bdaiface.h
api_name:
 - IBDA_Topology.GetNodeDescriptors
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBDA_Topology::GetNodeDescriptors


## -description



The <b>GetNodeDescriptors</b> method retrieves a list of descriptors for the nodes in the topology.




## -parameters




### -param ulcNodeDescriptors [in, out]

Receives a count of the number of node descriptors written to the <i>rgNodeDescriptors</i> array.


### -param ulcNodeDescriptorsMax [in]

Specifies the maximum number of node descriptors that the <i>rgNodeDescriptors</i> array can hold.


### -param rgNodeDescriptors [in, out]

Pointer to a buffer that receives an array of node descriptors. Each node descriptor is a structure of type <a href="https://msdn.microsoft.com/6ab03494-6564-4d4d-83bf-a9a6e588aac3">BDANODE_DESCRIPTOR</a>.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd693447(v=VS.85).aspx">IBDA_Topology Interface</a>
 

 

