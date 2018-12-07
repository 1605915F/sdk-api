---
UID: NE:resapi._RESOURCE_EXIT_STATE
title: "_RESOURCE_EXIT_STATE"
author: windows-sdk-content
description: Enumerates the possible exit states of a resource.
old-location: mscs\resource_exit_state.htm
tech.root: mscs
ms.assetid: d1b9fd8f-7d49-4396-8f0c-6db8fad5749e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: RESOURCE_EXIT_STATE, RESOURCE_EXIT_STATE enumeration [Failover Cluster], ResourceExitStateContinue, ResourceExitStateMax, ResourceExitStateTerminate, _RESOURCE_EXIT_STATE, mscs.resource_exit_state, resapi/RESOURCE_EXIT_STATE, resapi/ResourceExitStateContinue, resapi/ResourceExitStateMax, resapi/ResourceExitStateTerminate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: resapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Enterprise, Windows Server 2008 Datacenter
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
 - HeaderDef
api_location:
 - ResApi.h
api_name:
 - RESOURCE_EXIT_STATE
product: Windows
targetos: Windows
req.typenames: RESOURCE_EXIT_STATE
req.redist: 
---

# _RESOURCE_EXIT_STATE enumeration


## -description


Enumerates the possible exit states of a 
    <a href="https://msdn.microsoft.com/090d1c20-fab3-43dd-bfe2-a2c3f9ba8f89">resource</a>. These values are returned by the 
    <a href="https://msdn.microsoft.com/8ddb4578-f8c4-462e-af04-8c537d585e8b">SetResourceStatus</a> callback function.


## -enum-fields




### -field ResourceExitStateContinue

The resource has not been terminated. Worker threads may continue 
       <a href="https://msdn.microsoft.com/b406ef44-0622-4625-a6cf-462b6ea6018d">Online</a> and 
       <a href="https://msdn.microsoft.com/1d67a4f5-66f8-4818-8b63-d0f50452f889">Offline</a> operations for the resource.


### -field ResourceExitStateTerminate

The resource has been terminated. Callers should end 
       <a href="https://msdn.microsoft.com/b406ef44-0622-4625-a6cf-462b6ea6018d">Online</a> or 
       <a href="https://msdn.microsoft.com/1d67a4f5-66f8-4818-8b63-d0f50452f889">Offline</a> operations and immediately terminate all worker 
       threads assigned to the resource.


### -field ResourceExitStateMax

This value is only used for comparisons. All supported values are less than 
      <b>ResourceExitStateMax</b>.


## -see-also




<a href="https://msdn.microsoft.com/546071de-1067-4b47-b862-668be976e563">Failover Cluster Enumerations</a>



<a href="https://msdn.microsoft.com/8ddb4578-f8c4-462e-af04-8c537d585e8b">SetResourceStatus</a>
 

 

