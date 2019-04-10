---
UID: NF:gpmgmt.IGPMSOM.GetGPOLinks
title: IGPMSOM::GetGPOLinks (gpmgmt.h)
author: windows-sdk-content
description: Returns a GPMGPOLinksCollection object that contains the GPO links for the scope of management (SOM). The collection is sorted in the SOM link order and contains both enabled and disabled links. See IGPMGPOLink for the definition of SOM link order.
old-location: gpmc\igpmsom_getgpolinks.htm
tech.root: gpmc
ms.assetid: cab93e8e-d91d-47b6-9b33-adcf06fb9e41
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GPMSOM class [GPMC],GetGPOLinks method, GetGPOLinks, GetGPOLinks method [GPMC], GetGPOLinks method [GPMC],GPMSOM class, GetGPOLinks method [GPMC],IGPMSOM interface, IGPMSOM interface [GPMC],GetGPOLinks method, IGPMSOM.GetGPOLinks, IGPMSOM::GetGPOLinks, _win32_igpmsom_getgpolinks, gpmc.igpmsom_getgpolinks, gpmgmt/IGPMSOM::GetGPOLinks
ms.topic: method
req.header: gpmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Gpmgmt.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Gpmgmt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gpmgmt.dll
api_name:
 - IGPMSOM.GetGPOLinks
 - GPMSOM.GetGPOLinks
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IGPMSOM::GetGPOLinks


## -description


Returns a <a href="https://msdn.microsoft.com/37753a31-0ef8-4fb9-b542-a91ae47ed417">GPMGPOLinksCollection</a> object that contains the GPO links for the scope of management (SOM). The collection is sorted in the SOM link order and contains both enabled and disabled links. See <a href="https://msdn.microsoft.com/290a53fb-8be0-477d-837c-46251b30e245">IGPMGPOLink</a> for the definition of SOM link order.


## -parameters




### -param ppGPOLinks [out]

Address of a pointer to an 
<a href="https://msdn.microsoft.com/37753a31-0ef8-4fb9-b542-a91ae47ed417">IGPMGPOLinksCollection</a> interface.


## -returns



<h3>C++</h3>
Returns <b>S_OK</b> if successful. Returns a failure code if an error occurs.

<h3>JScript</h3>
Returns a reference to a <a href="https://msdn.microsoft.com/37753a31-0ef8-4fb9-b542-a91ae47ed417">GPMGPOLinksCollection</a> object.

<h3>VB</h3>
Returns a reference to a <a href="https://msdn.microsoft.com/37753a31-0ef8-4fb9-b542-a91ae47ed417">GPMGPOLinksCollection</a> object.




## -see-also




<a href="https://msdn.microsoft.com/290a53fb-8be0-477d-837c-46251b30e245">IGPMGPOLink</a>



<a href="https://msdn.microsoft.com/37753a31-0ef8-4fb9-b542-a91ae47ed417">IGPMGPOLinksCollection</a>



<a href="https://msdn.microsoft.com/e3252dba-403d-486d-b666-9bb04ec0aa90">IGPMSOM</a>
 

 

