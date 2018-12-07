---
UID: NF:comadmin.ICOMAdminCatalog2.GetComponentVersionCount
title: ICOMAdminCatalog2::GetComponentVersionCount
author: windows-sdk-content
description: Retrieves the number of partitions in which a specified component is installed.
old-location: cos\icomadmincatalog2_getcomponentversioncount.htm
tech.root: cossdk
ms.assetid: 5bbae408-3dbe-4f8f-92db-9ea1b8abd9ce
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetComponentVersionCount, GetComponentVersionCount method [COM+], GetComponentVersionCount method [COM+],ICOMAdminCatalog2 interface, ICOMAdminCatalog2 interface [COM+],GetComponentVersionCount method, ICOMAdminCatalog2.GetComponentVersionCount, ICOMAdminCatalog2::GetComponentVersionCount, _cos_icomadmincatalog2_GetComponentVersionCount, comadmin/ICOMAdminCatalog2::GetComponentVersionCount, cos.icomadmincatalog2_getcomponentversioncount
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: comadmin.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ComAdmin.Idl
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
 - ComAdmin.h
api_name:
 - ICOMAdminCatalog2.GetComponentVersionCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICOMAdminCatalog2::GetComponentVersionCount


## -description


Retrieves the number of partitions in which a specified component is installed.


## -parameters




### -param bstrCLSIDOrProgID [in]

The class ID or program ID of the component.


### -param plVersionCount [out, retval]

The number of different partitions in which the component is installed.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, E_UNEXPECTED, E_FAIL, and S_OK.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ee309562(v=VS.85).aspx">ICOMAdminCatalog2</a>
 

 

