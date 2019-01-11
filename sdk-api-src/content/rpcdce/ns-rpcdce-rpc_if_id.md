---
UID: NS:rpcdce._RPC_IF_ID
title: RPC_IF_ID
author: windows-sdk-content
description: The RPC_IF_ID structure contains the interface UUID and major and minor version numbers of an interface.
old-location: rpc\rpc_if_id.htm
tech.root: rpc
ms.assetid: 6fad80e0-4239-48f7-9cd1-3b9c56303346
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: RPC_IF_ID, RPC_IF_ID structure [RPC], _rpc_rpc_if_id, rpc.rpc_if_id, rpcdce/RPC_IF_ID
ms.topic: struct
req.header: rpcdce.h
req.include-header: Rpc.h
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
 - HeaderDef
api_location:
 - Rpcdce.h
api_name:
 - RPC_IF_ID
product: Windows
targetos: Windows
req.typenames: RPC_IF_ID
req.redist: 
---

# RPC_IF_ID structure


## -description


The 
<b>RPC_IF_ID</b> structure contains the interface UUID and major and minor version numbers of an interface.


## -struct-fields




### -field Uuid

Specifies the interface 
<a href="https://msdn.microsoft.com/72cf12f5-49cd-440d-9665-73211509d050">UUID</a>.


### -field VersMajor

Major version number, an integer from 0 to 65535, inclusive.


### -field VersMinor

Minor version number, an integer from 0 to 65535, inclusive.


## -remarks



An interface identification is a subset of the data contained in the interface-specification structure. Routines that require an interface identification structure show a data type of 
<b>RPC_IF_ID</b>. In those routines, the application is responsible for providing memory for the structure.




## -see-also




<a href="https://msdn.microsoft.com/1b91e88c-b242-472f-b719-60f96599cb67">RpcIfInqId</a>
 

 

