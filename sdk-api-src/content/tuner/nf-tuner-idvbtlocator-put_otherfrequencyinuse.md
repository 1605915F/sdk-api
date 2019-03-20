---
UID: NF:tuner.IDVBTLocator.put_OtherFrequencyInUse
title: IDVBTLocator::put_OtherFrequencyInUse (tuner.h)
author: windows-sdk-content
description: The put_OtherFrequencyInUse method specifies whether the frequency is being used by another DVB-T broadcaster.
old-location: mstv\idvbtlocator_put_otherfrequencyinuse.htm
tech.root: mstv
ms.assetid: ab9504f9-469d-476d-aad8-f9534f6b41bf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDVBTLocator interface [Microsoft TV Technologies],put_OtherFrequencyInUse method, IDVBTLocator.put_OtherFrequencyInUse, IDVBTLocator::put_OtherFrequencyInUse, IDVBTLocatorput_OtherFrequencyInUse, mstv.idvbtlocator_put_otherfrequencyinuse, put_OtherFrequencyInUse, put_OtherFrequencyInUse method [Microsoft TV Technologies], put_OtherFrequencyInUse method [Microsoft TV Technologies],IDVBTLocator interface, tuner/IDVBTLocator::put_OtherFrequencyInUse
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
 - IDVBTLocator.put_OtherFrequencyInUse
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDVBTLocator::put_OtherFrequencyInUse


## -description



The <b>put_OtherFrequencyInUse</b> method specifies whether the frequency is being used by another DVB-T broadcaster.




## -parameters




### -param OtherFrequencyInUseVal [in]

Specify VARIANT_TRUE if the frequency is being used by another DVB-T broadcaster, or VARIANT_FALSE otherwise.


## -returns



Returns S_OK if successful. If the method fails, error information can be retrieved using the standard COM <b>IErrorInfo</b> interface.




## -see-also




<a href="https://msdn.microsoft.com/f5a95a68-fee0-404c-b9c6-6b808977f8d2">IDVBTLocator Interface</a>
 

 

