---
UID: NF:objidlbase.IPSFactoryBuffer.CreateProxy
title: IPSFactoryBuffer::CreateProxy (objidlbase.h)
author: windows-sdk-content
description: Creates a proxy for the specified remote interface.
old-location: com\ipsfactorybuffer_createproxy.htm
tech.root: com
ms.assetid: 7d0638d9-50bc-47f3-8ebd-47bb5cbcab9c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CreateProxy, CreateProxy method [COM], CreateProxy method [COM],IPSFactoryBuffer interface, IPSFactoryBuffer interface [COM],CreateProxy method, IPSFactoryBuffer.CreateProxy, IPSFactoryBuffer::CreateProxy, _com_ipsfactorybuffer_createproxy, com.ipsfactorybuffer_createproxy, objidlbase/IPSFactoryBuffer::CreateProxy
ms.topic: method
req.header: objidlbase.h
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
 - objidlbase.h
api_name:
 - IPSFactoryBuffer.CreateProxy
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPSFactoryBuffer::CreateProxy


## -description


Creates a proxy for the specified remote interface.


## -parameters




### -param pUnkOuter [in]

A controlling <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface; used for aggregation.


### -param riid [in]

The identifier of the interface to proxy.


### -param ppProxy [out]

A pointer to an <a href="https://msdn.microsoft.com/e1b18997-f99b-4611-8ba6-da28fd8df898">IRpcProxyBuffer</a> interface to control marshaling.


### -param ppv [out]

A pointer to the interface specified by <i>riid</i>.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, E_UNEXPECTED, E_FAIL, and S_OK.




## -remarks



The <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> implementation of the <a href="https://msdn.microsoft.com/e1b18997-f99b-4611-8ba6-da28fd8df898">IRpcProxyBuffer</a> interface must not delegate to the outer controlling <b>IUnknown</b>.




## -see-also




<a href="https://msdn.microsoft.com/ffe85701-a4fa-4cf3-9b86-85f3a0cb63e9">IPSFactoryBuffer</a>



<a href="https://msdn.microsoft.com/e1b18997-f99b-4611-8ba6-da28fd8df898">IRpcProxyBuffer</a>



<a href="https://msdn.microsoft.com/6c82f655-ac46-4ed9-992b-0387b324a8f9">Proxy</a>
 

 

