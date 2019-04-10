---
UID: NF:webservices.WsFindAttribute
title: WsFindAttribute function (webservices.h)
author: windows-sdk-content
description: Searches the attributes of the current element for an attribute with the specified name and namespace and returns its index which may be passed to WsReadStartAttribute.
old-location: wsw\wsfindattribute.htm
tech.root: wsw
ms.assetid: beb00382-6cc0-42c6-b835-4ebc94c5faa2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WsFindAttribute, WsFindAttribute function [Web Services for Windows], webservices/WsFindAttribute, wsw.wsfindattribute
ms.topic: function
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
req.lib: WebServices.lib
req.dll: WebServices.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - WebServices.dll
api_name:
 - WsFindAttribute
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WsFindAttribute function


## -description


Searches the attributes of the current element for an attribute with the 
        specified name and namespace and returns its index which may be passed 
        to <a href="https://msdn.microsoft.com/6fd0c8c2-2eac-4d98-898d-1c5849220c36">WsReadStartAttribute</a>.
      


## -parameters




### -param reader [in]

The reader on which to find the attribute.
        


### -param localName [in]

The local name of the attribute to search for.
        


### -param ns [in]

The namespace of the attribute to search for.
        


### -param required [in]

If required is <b>TRUE</b> and the attribute is not found,  the function will return <b>WS_E_INVALID_FORMAT</b>.
          (See <a href="https://msdn.microsoft.com/96285557-8317-4875-b634-e2eacd605901">Windows Web Services Return Values</a>.) if required is <b>FALSE</b> and the attribute is not found, the function will return S_FALSE.
        


### -param attributeIndex [out]

If the attribute is found, then the index of the attribute, is returned here.
          This index can then be passed to <a href="https://msdn.microsoft.com/6fd0c8c2-2eac-4d98-898d-1c5849220c36">WsReadStartAttribute</a>.
        


### -param error [in, optional]

Specifies where additional error information should be stored if the function fails.
        


## -returns



This function can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WS_E_INVALID_FORMAT</b></dt>
</dl>
</td>
<td width="60%">
The input data was not in the expected format or did not have the expected value.

</td>
</tr>
</table>
 




## -remarks



If the reader is not positioned on a start element then it will return <b>WS_E_INVALID_OPERATION</b>.
      (See <a href="https://msdn.microsoft.com/96285557-8317-4875-b634-e2eacd605901">Windows Web Services Return Values</a>.) 

The index returned does not necessarily correspond to the position of the attribute as it appeared
        in the document.  It identifies the index of the matching attribute in the array of attributes of
        the <a href="https://msdn.microsoft.com/32157ddf-ace2-49dc-85d7-b04e25e85693">WS_XML_ELEMENT_NODE</a>.  The order of the attributes in this array may differ from the order
        in which the attributes appeared in the document.
      



