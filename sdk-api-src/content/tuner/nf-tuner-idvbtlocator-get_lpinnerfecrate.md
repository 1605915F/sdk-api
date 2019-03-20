---
UID: NF:tuner.IDVBTLocator.get_LPInnerFECRate
title: IDVBTLocator::get_LPInnerFECRate (tuner.h)
author: windows-sdk-content
description: The get_LPInnerFECRate method retrieves the inner FEC rate of the low-priority stream.
old-location: mstv\idvbtlocator_get_lpinnerfecrate.htm
tech.root: mstv
ms.assetid: eeed8fe6-774d-4375-9b3c-ebe979cd11dd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDVBTLocator interface [Microsoft TV Technologies],get_LPInnerFECRate method, IDVBTLocator.get_LPInnerFECRate, IDVBTLocator::get_LPInnerFECRate, IDVBTLocatorget_LPInnerFECRate, get_LPInnerFECRate, get_LPInnerFECRate method [Microsoft TV Technologies], get_LPInnerFECRate method [Microsoft TV Technologies],IDVBTLocator interface, mstv.idvbtlocator_get_lpinnerfecrate, tuner/IDVBTLocator::get_LPInnerFECRate
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
 - tuner.h
api_name:
 - IDVBTLocator.get_LPInnerFECRate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDVBTLocator::get_LPInnerFECRate


## -description



The <b>get_LPInnerFECRate</b> method retrieves the inner FEC rate of the low-priority stream.




## -parameters




### -param FEC [out]

Receives a member of the <a href="https://msdn.microsoft.com/161c963f-55b2-4a17-a537-47de3326df0e">BinaryConvolutionCodeRate</a> enumeration.


## -returns



Returns S_OK if successful. If the method fails, error information can be retrieved using the standard COM <b>IErrorInfo</b> interface.




## -see-also




<a href="https://msdn.microsoft.com/f5a95a68-fee0-404c-b9c6-6b808977f8d2">IDVBTLocator Interface</a>
 

 

