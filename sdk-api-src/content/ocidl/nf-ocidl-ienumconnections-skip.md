---
UID: NF:ocidl.IEnumConnections.Skip
title: IEnumConnections::Skip (ocidl.h)
author: windows-sdk-content
description: Skips over the specified number of items in the enumeration sequence.
old-location: com\ienumconnections_skip.htm
tech.root: com
ms.assetid: bf875481-74cf-4e29-af81-b1546fb00002
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IEnumConnections interface [COM],Skip method, IEnumConnections.Skip, IEnumConnections::Skip, Skip, Skip method [COM], Skip method [COM],IEnumConnections interface, _com_ienumconnections_skip, com.ienumconnections_skip, ocidl/IEnumConnections::Skip
ms.topic: method
req.header: ocidl.h
req.include-header: ObjIdl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ObjIdl.idl
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
 - ocidl.h
api_name:
 - IEnumConnections.Skip
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumConnections::Skip


## -description


Skips over the specified number of items in the enumeration sequence.


## -parameters




### -param cConnections [in]

The number of items to be skipped.


## -returns



If the method skips the number of items requested, the return value is S_OK. Otherwise, it is S_FALSE.




## -see-also




<a href="https://msdn.microsoft.com/464966c1-e4e9-4b58-9e41-48de408f572f">IEnumConnections</a>
 

 

