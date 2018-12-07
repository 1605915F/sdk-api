---
UID: NS:wsdtypes._WSD_OPERATION
title: "_WSD_OPERATION"
author: windows-sdk-content
description: Describes an operation as defined by WSDL in terms of one or two messages.
old-location: ncd\wsd_operation_struct.htm
tech.root: wsdapi
ms.assetid: fcd4895d-5357-4b73-90b9-e506e3d7f16e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WSD_OPERATION, WSD_OPERATION structure, _WSD_OPERATION, ncd.wsd_operation_struct, wsdtypes/WSD_OPERATION
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - WSD_OPERATION
product: Windows
targetos: Windows
req.typenames: WSD_OPERATION
req.redist: 
---

# _WSD_OPERATION structure


## -description


Describes an operation as defined by WSDL in terms of one or two messages. This structure is populated by <a href="https://msdn.microsoft.com/76dffca8-bb84-4384-a9e8-120a4cf2acac">generated code</a>.


## -struct-fields




### -field RequestType

Reference to a <a href="https://msdn.microsoft.com/dc214dfb-1717-4f84-af4d-6eb8cf17522c">WSDXML_TYPE</a> structure that specifies the request type of an incoming message.


### -field ResponseType

Reference to a <a href="https://msdn.microsoft.com/dc214dfb-1717-4f84-af4d-6eb8cf17522c">WSDXML_TYPE</a> structure that specifies the response type of an outgoing message.


### -field RequestStubFunction

Reference to a <a href="https://msdn.microsoft.com/39d16b22-2af0-43e4-a0d2-ca5e1d3a9434">WSD_STUB_FUNCTION</a> function that specifies the address of a stub function which translates a generic SOAP message structure into a method call with a signature specific to the incoming message of the operation. 


