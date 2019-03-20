---
UID: NF:ocidl.IEnumConnectionPoints.Next
title: IEnumConnectionPoints::Next (ocidl.h)
author: windows-sdk-content
description: Retrieves the specified number of items in the enumeration sequence.
old-location: com\ienumconnectionpoints_next.htm
tech.root: com
ms.assetid: 954bd587-75ce-4216-85c9-f1382414a979
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumConnectionPoints interface [COM],Next method, IEnumConnectionPoints.Next, IEnumConnectionPoints::Next, Next, Next method [COM], Next method [COM],IEnumConnectionPoints interface, _com_ienumconnectionpoints_next, com.ienumconnectionpoints_next, ocidl/IEnumConnectionPoints::Next
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
 - IEnumConnectionPoints.Next
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumConnectionPoints::Next


## -description


Retrieves the specified number of items in the enumeration sequence.


## -parameters




### -param cConnections [in]

The number of items to be retrieved. If there are fewer than the requested number of items left in the sequence, this method retrieves the remaining elements.


### -param ppCP [out]

An array of enumerated items.

The enumerator is responsible for calling <a href="https://msdn.microsoft.com/b4316efd-73d4-4995-b898-8025a316ba63">AddRef</a>, and the caller is responsible for calling <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">Release</a> through each pointer enumerated. If <i>cConnections</i> is greater than 1, the caller must also pass a non-NULL pointer passed to <i>lpcFetched</i> to know how many pointers to release.


### -param pcFetched [out]

The number of items that were retrieved. This parameter is always less than or equal to the number of items requested.


## -returns



If the method retrieves the number of items requested, the return value is S_OK. Otherwise, it is S_FALSE.




## -see-also




<a href="https://msdn.microsoft.com/ef5a917c-b57f-4000-8daa-86fdbfb47579">IConnectionPoint</a>



<a href="https://msdn.microsoft.com/893090f1-a0b4-46f1-a5d0-1da704ca7aa9">IEnumConnectionPoints</a>
 

 

