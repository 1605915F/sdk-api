---
UID: NF:bdatif.IGuideDataEvent.GuideDataAcquired
title: IGuideDataEvent::GuideDataAcquired (bdatif.h)
author: windows-sdk-content
description: The GuideDataAcquired method is called when a complete set of guide data has been acquired from the current transport stream.
old-location: mstv\iguidedataevent_guidedataacquired.htm
tech.root: mstv
ms.assetid: 00f1aec7-4d26-4323-9d7e-c75d9a0c374c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GuideDataAcquired, GuideDataAcquired method [Microsoft TV Technologies], GuideDataAcquired method [Microsoft TV Technologies],IGuideDataEvent interface, IGuideDataEvent interface [Microsoft TV Technologies],GuideDataAcquired method, IGuideDataEvent.GuideDataAcquired, IGuideDataEvent::GuideDataAcquired, IGuideDataEventGuideDataAcquired, bdatif/IGuideDataEvent::GuideDataAcquired, mstv.iguidedataevent_guidedataacquired
ms.topic: method
req.header: bdatif.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - bdatif.h
api_name:
 - IGuideDataEvent.GuideDataAcquired
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IGuideDataEvent::GuideDataAcquired


## -description



The <b>GuideDataAcquired</b> method is called when a complete set of guide data has been acquired from the current transport stream.



Currently the <a href="https://msdn.microsoft.com/22044a4c-480f-4c98-a78e-52c66a5eac99">BDA MPEG-2 Transport Information Filter</a> (TIF) does not support this event, so this method is not called.


## -parameters






## -returns



Return S_OK if successful, or an error code.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/9da565f2-fbcb-4d71-ae40-7d9821f46630">IGuideDataEvent Interface</a>
 

 

