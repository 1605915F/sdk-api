---
UID: NF:mfmediaengine.IMFMediaEngineClassFactory.CreateTimeRange
title: IMFMediaEngineClassFactory::CreateTimeRange
author: windows-sdk-content
description: Creates a time range object.
old-location: mf\imfmediaengineclassfactory_createtimerange.htm
tech.root: medfound
ms.assetid: 293769E8-8C8A-40D1-AF51-1DBB773F88D5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateTimeRange, CreateTimeRange method [Media Foundation], CreateTimeRange method [Media Foundation],IMFMediaEngineClassFactory interface, IMFMediaEngineClassFactory interface [Media Foundation],CreateTimeRange method, IMFMediaEngineClassFactory.CreateTimeRange, IMFMediaEngineClassFactory::CreateTimeRange, mf.imfmediaengineclassfactory_createtimerange, mfmediaengine/IMFMediaEngineClassFactory::CreateTimeRange
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mfmediaengine.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
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
 - mfmediaengine.h
api_name:
 - IMFMediaEngineClassFactory.CreateTimeRange
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFMediaEngineClassFactory::CreateTimeRange


## -description


Creates a time range object.


## -parameters




### -param ppTimeRange [out]

Receives a pointer to the <a href="https://msdn.microsoft.com/E39646E6-66F4-4413-A84B-43039689AEE7">IMFMediaTimeRange</a> interface. The caller must release the interface.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/8E4E84A0-BCFC-4CBF-813B-4FEE2B42A83E">IMFMediaEngineClassFactory</a>
 

 

