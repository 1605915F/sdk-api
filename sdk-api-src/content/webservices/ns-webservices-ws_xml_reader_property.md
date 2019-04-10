---
UID: NS:webservices._WS_XML_READER_PROPERTY
title: WS_XML_READER_PROPERTY (webservices.h)
author: windows-sdk-content
description: Specifies a reader specific setting.
old-location: wsw\ws_xml_reader_property.htm
tech.root: wsw
ms.assetid: 8864d679-c321-45bb-b774-f05696d6098e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WS_XML_READER_PROPERTY, WS_XML_READER_PROPERTY structure [Web Services for Windows], webservices/WS_XML_READER_PROPERTY, wsw.ws_xml_reader_property
ms.topic: struct
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - WS_XML_READER_PROPERTY
product: Windows
targetos: Windows
req.typenames: WS_XML_READER_PROPERTY
req.redist: 
---

# WS_XML_READER_PROPERTY structure


## -description


Specifies a reader specific setting.
      


## -struct-fields




### -field id

Identifies the <a href="https://msdn.microsoft.com/b8d36716-e25a-4215-8bc7-30091b68c0f6">WS_XML_READER_PROPERTY_ID</a>.
        


### -field value

A pointer to the value to set.
            The pointer must have an alignment compatible with the type
            of the property.
        


### -field valueSize

The size in bytes of the memory pointed to by value.
        

