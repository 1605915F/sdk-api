---
UID: NF:iads.IADsPrintQueueOperations.PrintJobs
title: IADsPrintQueueOperations::PrintJobs
author: windows-sdk-content
description: The IADsPrintQueueOperations::PrintJobs method gets an IADsCollection interface pointer on the collection of the print jobs processed in this print queue.
old-location: adsi\iadsprintqueueoperations_printjobs.htm
tech.root: adsi
ms.assetid: fe92fef3-596f-416c-b613-1d93737c298e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IADsPrintQueueOperations interface [ADSI],PrintJobs method, IADsPrintQueueOperations.PrintJobs, IADsPrintQueueOperations::PrintJobs, PrintJobs, PrintJobs method [ADSI], PrintJobs method [ADSI],IADsPrintQueueOperations interface, _ds_iadsprintqueueoperations_printjobs, adsi.iadsprintqueueoperations__printjobs, adsi.iadsprintqueueoperations_printjobs, iads/IADsPrintQueueOperations::PrintJobs
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: iads.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Activeds.dll
api_name:
 - IADsPrintQueueOperations.PrintJobs
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsPrintQueueOperations::PrintJobs


## -description


The <b>IADsPrintQueueOperations::PrintJobs</b> method gets an  <a href="https://msdn.microsoft.com/4552552b-c008-439a-95bf-eaf9ffd28b5f">IADsCollection</a> interface pointer on the collection of the print jobs processed in this print queue. This collection can be enumerated using the standard Automation enumeration methods on  <a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a>. To delete a print job, use the  <a href="https://msdn.microsoft.com/21ce80fe-542b-4350-b66c-fa26f62ca611">IADsCollection::Remove</a> method on the retrieved interface pointer.


## -parameters




### -param pObject [out]

Pointer to a pointer to the  <a href="https://msdn.microsoft.com/4552552b-c008-439a-95bf-eaf9ffd28b5f">IADsCollection</a> interface on the collection of objects added to this print queue. Objects in the collection implement the  <a href="https://msdn.microsoft.com/82d61e39-4dbb-41c9-85d5-6f4e7ab7f66b">IADsPrintJob</a> interface.


## -returns



This method supports the standard return values. For more information about other return values, see the  <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/9bfc98a5-f4f0-4127-89c9-b8ed01bfde4e">ADsEnumerateNext</a>



<a href="https://msdn.microsoft.com/4552552b-c008-439a-95bf-eaf9ffd28b5f">IADsCollection</a>



<a href="https://msdn.microsoft.com/21ce80fe-542b-4350-b66c-fa26f62ca611">IADsCollection::Remove</a>



<a href="https://msdn.microsoft.com/82d61e39-4dbb-41c9-85d5-6f4e7ab7f66b">IADsPrintJob</a>



<a href="https://msdn.microsoft.com/23e7cbf3-09ce-44ce-b618-2c0fa6b34428">IADsPrintJob Property Methods</a>



<a href="https://msdn.microsoft.com/97495455-a576-4984-beb8-9282073e88c2">IADsPrintQueueOperations</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a>
 

 

