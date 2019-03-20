---
UID: NC:routprot.PMIB_SET
title: PMIB_SET (routprot.h)
author: windows-sdk-content
description: The MibSet function passes a SNMP MIB-style Set Request to the routing protocol.
old-location: rras\mibset.htm
tech.root: RRAS
ms.assetid: f1df3476-f6c5-4f7e-bc86-83e5f8d0cd57
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MibSet, PMIB_SET, PMIB_SET callback, PMIB_SET callback function [RAS], TBD, _mpr_mibset, routprot/PMIB_SET, rras.mibset
ms.topic: callback
req.header: routprot.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
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
 - UserDefined
api_location:
 - Routprot.h
api_name:
 - PMIB_SET
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PMIB_SET callback function


## -description


The 
<b>MibSet</b> function passes a SNMP MIB-style Set Request to the routing protocol.


## -parameters




### -param InputDataSize [in]

Specifies the size of the data for the Set Request.


### -param InputData [in]

Pointer to a buffer that specifies the data for the Set Request.


## -returns



If the function succeeds, the return value is NO_ERROR.

If the function fails, the return value is one of the following error codes.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_CAN_NOT_COMPLETE</b></dt>
</dl>
</td>
<td width="60%">
The routing protocol could not complete the request.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The size or content of the data is inappropriate for the request.

</td>
</tr>
</table>
 


<div> </div>





## -see-also




<a href="https://msdn.microsoft.com/a6f3d450-0ca1-4c22-9e48-addf317cac2a">MibGet</a>



<a href="https://msdn.microsoft.com/3aef09e2-6314-4de8-a9dd-e02c13e0145c">MibGetFirst</a>



<a href="https://msdn.microsoft.com/00047426-11b6-4b68-8a44-45608611eafe">MibGetNext</a>



<a href="https://msdn.microsoft.com/fd780458-ef23-4ef2-8fe8-29b32100917f">Routing Protocol Interface Functions</a>



<a href="https://msdn.microsoft.com/0429f5ca-6574-48f5-85ab-70b4677ca539">Routing Protocol Interface Reference</a>
 

 

