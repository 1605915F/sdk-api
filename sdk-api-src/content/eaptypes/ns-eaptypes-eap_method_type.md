---
UID: NS:eaptypes._EAP_METHOD_TYPE
title: EAP_METHOD_TYPE (eaptypes.h)
author: windows-sdk-content
description: Contains type, identification, and author information about an EAP method.
old-location: eaphost\eap_method_type.htm
tech.root: eaphost
ms.assetid: 47702dd9-d9c2-4dd5-a12d-23a55b031d27
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EAP_METHOD_TYPE, EAP_METHOD_TYPE structure [EAPHost], eaphost.eap_method_type, eaptypes/EAP_METHOD_TYPE
ms.topic: struct
req.header: eaptypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - HeaderDef
api_location:
 - eaptypes.h
api_name:
 - EAP_METHOD_TYPE
product: Windows
targetos: Windows
req.typenames: EAP_METHOD_TYPE
req.redist: 
---

# EAP_METHOD_TYPE structure


## -description


The <b>EAP_METHOD_TYPE</b> structure contains  type, identification, and author information about an EAP method.


## -struct-fields




### -field eapType


<a href="https://msdn.microsoft.com/383f1e11-2e40-45e6-8c55-a23d1b8eb71f">EAP_TYPE</a> structure that contains the ID for the EAP method as well as specific vendor information.


### -field dwAuthorId

The numeric ID for the author of the EAP method.


## -see-also




<a href="https://msdn.microsoft.com/f6f3b909-1e89-47f8-853c-c0f3f2414817">Common EAPHost API Structures</a>



<a href="https://msdn.microsoft.com/383f1e11-2e40-45e6-8c55-a23d1b8eb71f">EAP_TYPE</a>
 

 

