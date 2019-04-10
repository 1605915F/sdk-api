---
UID: NF:manipulations.IInertiaProcessor.Complete
title: IInertiaProcessor::Complete (manipulations.h)
author: windows-sdk-content
description: The Complete method finishes the current manipulation and stops inertia on the inertia processor.
old-location: wintouch\iinertiaprocessor_complete.htm
tech.root: wintouch
ms.assetid: ff41789c-afc5-419b-9767-e99572b9b41e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Complete, Complete method [Windows Touch], Complete method [Windows Touch],IInertiaProcessor interface, IInertiaProcessor interface [Windows Touch],Complete method, IInertiaProcessor.Complete, IInertiaProcessor::Complete, manipulations/IInertiaProcessor::Complete, wintouch.iinertiaprocessor_complete
ms.topic: method
req.header: manipulations.h
req.include-header: Manipulations.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - manipulations.h
api_name:
 - IInertiaProcessor.Complete
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInertiaProcessor::Complete


## -description


The <b>Complete</b> method finishes the current manipulation and stops inertia on the inertia processor.


## -parameters






## -returns



Returns <b>S_OK</b> on success, otherwise returns an error code such as <b>E_FAIL</b>.




## -remarks



The <b>Complete</b> method raises the <a href="https://msdn.microsoft.com/1284df32-f4e8-43b3-b825-9172ad39f0e6">ManipulationCompleted</a> event	on an <a href="https://msdn.microsoft.com/be392a13-3165-44ff-bcd6-ed0075c669c4">_IManipulationEvents</a> interface implementation.
	 


#### Examples


```cpp

    // set properties on the IInertiaProcessor interface
    this->m_spIInertProc->put_DesiredRotation(spin);    
	 
    // complete any unprocessed inertia
    this->m_spIInertProc->Complete();
	 
    // reset the processor
    this->m_spIInertProc->Reset();		  
	 
    // If you have implemented a timer that handles inertia processing,
    // this should be started as well and the processor will raise
    // Manipulation* events
		  
```





## -see-also




<a href="https://msdn.microsoft.com/325e04c2-a477-43c7-9513-36a2a92eef8e">CompleteTime</a>



<a href="https://msdn.microsoft.com/8dc171eb-0c6e-41dd-b506-5f91ea703a53">IInertiaProcessor</a>



<a href="https://msdn.microsoft.com/e4acfcac-06c1-42a5-9722-4534a4492ab8">Methods</a>
 

 

