---
UID: NS:wsdtypes._WSD_BYE
title: WSD_BYE (wsdtypes.h)
author: windows-sdk-content
description: Represents a Bye message.
old-location: ncd\wsd_bye_struct.htm
tech.root: WsdApi
ms.assetid: b0eb67e1-1408-45ab-b7a7-ecde6619a277
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WSD_BYE, WSD_BYE structure, ncd.wsd_bye_struct, wsdtypes/WSD_BYE
ms.topic: struct
req.header: wsdtypes.h
req.include-header: Wsdapi.h
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
 - WsdTypes.h
api_name:
 - WSD_BYE
product: Windows
targetos: Windows
req.typenames: WSD_BYE
req.redist: 
---

# WSD_BYE structure


## -description


Represents a <a href="https://msdn.microsoft.com/7b9abfcc-28ab-4f29-af69-6dc68e3f51b6">Bye</a> message.


## -struct-fields




### -field EndpointReference

Reference to a <a href="https://msdn.microsoft.com/97d6870e-3633-4bea-9a50-984e6b0ba3a1">WSD_ENDPOINT_REFERENCE</a> structure that specifies either the sending or receiving endpoint of the Bye message. 


### -field Any

Reference to a <a href="https://msdn.microsoft.com/727149b4-31b0-4fd8-b0fa-eb773edb171e">WSDXML_ELEMENT</a> structure that specifies content allowed by the XML <b>ANY</b> keyword.


## -see-also




<a href="https://msdn.microsoft.com/7b9abfcc-28ab-4f29-af69-6dc68e3f51b6">Bye Message</a>
 

 

