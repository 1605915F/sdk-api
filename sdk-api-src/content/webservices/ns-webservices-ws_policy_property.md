---
UID: NS:webservices._WS_POLICY_PROPERTY
title: WS_POLICY_PROPERTY (webservices.h)
author: windows-sdk-content
description: Specifies a policy object setting.
old-location: wsw\ws_policy_property.htm
tech.root: wsw
ms.assetid: a897eb6c-d527-46ec-a710-252679001185
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WS_POLICY_PROPERTY, WS_POLICY_PROPERTY structure [Web Services for Windows], webservices/WS_POLICY_PROPERTY, wsw.ws_policy_property
ms.topic: struct
req.header: webservices.h
req.include-header: 
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
 - HeaderDef
api_location:
 - WebServices.h
api_name:
 - WS_POLICY_PROPERTY
product: Windows
targetos: Windows
req.typenames: WS_POLICY_PROPERTY
req.redist: 
---

# WS_POLICY_PROPERTY structure


## -description


Specifies a policy object setting.
            


## -struct-fields




### -field id

Identifies the <a href="https://msdn.microsoft.com/503d39c0-7546-429d-b8e3-66e80c76b7c1">WS_POLICY_PROPERTY_ID</a>.
                


### -field value

A pointer to the value to set.
                    The pointer must have an alignment compatible with the type
                    of the property.
                


### -field valueSize

The size in bytes of the memory pointed to by value.
                

