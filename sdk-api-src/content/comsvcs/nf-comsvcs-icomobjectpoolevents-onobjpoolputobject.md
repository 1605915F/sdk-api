---
UID: NF:comsvcs.IComObjectPoolEvents.OnObjPoolPutObject
title: IComObjectPoolEvents::OnObjPoolPutObject
author: windows-sdk-content
description: Generated when a new object is added to the pool.
old-location: cos\icomobjectpoolevents_onobjpoolputobject.htm
tech.root: cossdk
ms.assetid: 00b0b3b1-943d-4fba-bd5d-52d6de80fcf6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComObjectPoolEvents interface [COM+],OnObjPoolPutObject method, IComObjectPoolEvents.OnObjPoolPutObject, IComObjectPoolEvents::OnObjPoolPutObject, OnObjPoolPutObject, OnObjPoolPutObject method [COM+], OnObjPoolPutObject method [COM+],IComObjectPoolEvents interface, _dtc_IComObjectPoolEvents_OnObjPoolPutObject, comsvcs/IComObjectPoolEvents::OnObjPoolPutObject, cos.icomobjectpoolevents_onobjpoolputobject
ms.topic: method
req.header: comsvcs.h
req.include-header: 
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
 - COM
api_location:
 - ComSvcs.h
api_name:
 - IComObjectPoolEvents.OnObjPoolPutObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComObjectPoolEvents::OnObjPoolPutObject


## -description


Generated when a new object is added to the pool.


## -parameters




### -param pInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms688276(v=VS.85).aspx">COMSVCSEVENTINFO</a> structure.


### -param guidObject [in]

The CLSID for the objects in the pool.


### -param nReason [in]

This parameter is always 0.


### -param dwAvailable [in]

The number of objects in the pool.


### -param oid [in]

The unique identifier for this object.


## -returns



The user verifies the return values from this method.




## -see-also




<a href="https://msdn.microsoft.com/a830b40b-a1b1-464e-b532-91cebd4e5d2f">IComObjectPoolEvents</a>
 

 

