---
UID: NF:tuner.ITuner.put_TuneRequest
title: ITuner::put_TuneRequest
author: windows-sdk-content
description: The put_TuneRequest method sets the tune request currently in effect for the Network Provider.
old-location: mstv\ituner_put_tunerequest.htm
tech.root: mstv
ms.assetid: 69f71855-86d0-4ef9-a168-14e79461ec98
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITuner interface [Microsoft TV Technologies],put_TuneRequest method, ITuner.put_TuneRequest, ITuner::put_TuneRequest, ITunerput_TuneRequest, mstv.ituner_put_tunerequest, put_TuneRequest, put_TuneRequest method [Microsoft TV Technologies], put_TuneRequest method [Microsoft TV Technologies],ITuner interface, tuner/ITuner::put_TuneRequest
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - ITuner.put_TuneRequest
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITuner::put_TuneRequest


## -description



The <b>put_TuneRequest</b> method sets the tune request currently in effect for the Network Provider.




## -parameters




### -param TuneRequest [in]

Pointer to an <a href="https://msdn.microsoft.com/34077b45-32b4-466b-b103-6a42fc869265">ITuneRequest</a> object that will be used to set the Network Provider.


## -returns



When the method is successful, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code.




## -remarks



Calling this method initiates a tuning operation based on the properties of the tune request. The tuning operation may be asynchronously attempted.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/1bc965a5-6bc9-488a-a2f9-f35d0cfbcccd">ITuner Interface</a>
 

 

