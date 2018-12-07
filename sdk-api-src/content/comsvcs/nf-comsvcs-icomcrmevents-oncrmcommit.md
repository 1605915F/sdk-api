---
UID: NF:comsvcs.IComCRMEvents.OnCRMCommit
title: IComCRMEvents::OnCRMCommit
author: windows-sdk-content
description: Generated when CRM clerk receives a commit notification to pass on to the CRM compensator.
old-location: cos\icomcrmevents_oncrmcommit.htm
tech.root: cossdk
ms.assetid: 76b87452-fa29-49f7-acc8-2ae2039757b0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComCRMEvents interface [COM+],OnCRMCommit method, IComCRMEvents.OnCRMCommit, IComCRMEvents::OnCRMCommit, OnCRMCommit, OnCRMCommit method [COM+], OnCRMCommit method [COM+],IComCRMEvents interface, _dtc_IComCRMEvents_OnCRMCommit, comsvcs/IComCRMEvents::OnCRMCommit, cos.icomcrmevents_oncrmcommit
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IComCRMEvents.OnCRMCommit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComCRMEvents::OnCRMCommit


## -description


Generated when CRM clerk receives a commit notification to pass on to the CRM compensator.


## -parameters




### -param pInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/f4aa0892-4c93-42ea-adc6-1b304b917389">COMSVCSEVENTINFO</a> structure.


### -param guidClerkCLSID [in]

The identifier of the CRM clerk.


## -returns



The user verifies the return values from this method.




## -see-also




<a href="https://msdn.microsoft.com/720beffb-8fb5-4c87-9bcf-6db214543b01">IComCRMEvents</a>
 

 

