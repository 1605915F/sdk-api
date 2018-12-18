---
UID: NF:ehstorapi.IEnhancedStorageACT.Unauthorize
title: IEnhancedStorageACT::Unauthorize
author: windows-sdk-content
description: Associates the Addressable Command Target (ACT) with the Unauthorized state defined by ACT_AUTHORIZATION_STATE, and ensures the deauthentication of each individual silo according to the required sequence and logical combination necessary to restrict access to the ACT.
old-location: enstor\ienhancedstorageact_unauthorize.htm
tech.root: enstor
ms.assetid: 82f78f9d-fb50-4f44-b4ad-f3a43ccca671
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnhancedStorageACT interface [Enhanced Storage],Unauthorize method, IEnhancedStorageACT.Unauthorize, IEnhancedStorageACT::Unauthorize, Unauthorize, Unauthorize method [Enhanced Storage], Unauthorize method [Enhanced Storage],IEnhancedStorageACT interface, ehstorapi/IEnhancedStorageACT::Unauthorize, enstor.ienhancedstorageact_unauthorize
ms.topic: method
req.header: ehstorapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: EhStorAPI.idl
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
 - EhStorAPI.h
api_name:
 - IEnhancedStorageACT.Unauthorize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnhancedStorageACT::Unauthorize


## -description


Associates the Addressable Command Target (ACT) with the <b>Unauthorized</b> state defined by <a href="https://msdn.microsoft.com/385b2f9d-659e-451d-97da-15be70180e1f">ACT_AUTHORIZATION_STATE</a>, and ensures the deauthentication of each individual silo according to the required sequence and logical combination necessary to restrict access to the ACT.


## -parameters






## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK </b></dt>
</dl>
</td>
<td width="60%">
Unauthorization completed successfully.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/33d5df30-f877-4852-ad2f-af1bb58d0044">IEnhancedStorageACT</a>
 

 

