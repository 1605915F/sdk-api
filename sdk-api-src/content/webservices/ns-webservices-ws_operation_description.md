---
UID: NS:webservices._WS_OPERATION_DESCRIPTION
title: WS_OPERATION_DESCRIPTION (webservices.h)
author: windows-sdk-content
description: Metadata for the service operation.
old-location: wsw\ws_operation_description.htm
tech.root: wsw
ms.assetid: d05b55aa-4159-4e48-ae75-2af36c0a7101
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WS_OPERATION_DESCRIPTION, WS_OPERATION_DESCRIPTION structure [Web Services for Windows], webservices/WS_OPERATION_DESCRIPTION, wsw.ws_operation_description
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
 - WS_OPERATION_DESCRIPTION
product: Windows
targetos: Windows
req.typenames: WS_OPERATION_DESCRIPTION
req.redist: 
---

# WS_OPERATION_DESCRIPTION structure


## -description


Metadata for the  service operation.
            


## -struct-fields




### -field versionInfo

Defines the version information. Currently value is 1.
                


### -field inputMessageDescription

The description of incoming <a href="https://msdn.microsoft.com/22cc39a9-a3a7-4b4d-bdee-0ccac5dc03ee">WS_MESSAGE</a> for a given service operation.
                


### -field outputMessageDescription

The description of outgoing <a href="https://msdn.microsoft.com/22cc39a9-a3a7-4b4d-bdee-0ccac5dc03ee">WS_MESSAGE</a> for a given service operation. For one way operations this should be <b>NULL</b>.
                


### -field inputMessageOptions

Provides additional flags for the in message of the operation. See <a href="https://msdn.microsoft.com/3f54e012-4893-4f70-9f38-55ae9db365e8">WS_SERVICE_OPERATION_MESSAGE_OPTION</a> for
                    a list of flags. If no flags are needed, this may be 0.
                


<a href="https://msdn.microsoft.com/3f54e012-4893-4f70-9f38-55ae9db365e8">WS_SERVICE_OPERATION_MESSAGE_NILLABLE_ELEMENT</a> is not applicable to <a href="https://msdn.microsoft.com/c0cc2c3c-5050-444a-95e9-2cfb0e755253">WS_RPC_LITERAL_OPERATION</a> style
                    operations. The input parameter must be with type of <a href="https://msdn.microsoft.com/c847940a-f97e-4605-a940-1d72de6a3695">WS_PARAMETER_TYPE_MESSAGES</a>.
                


### -field outputMessageOptions

Provides additional flags for the out message of the operation. See <a href="https://msdn.microsoft.com/3f54e012-4893-4f70-9f38-55ae9db365e8">WS_SERVICE_OPERATION_MESSAGE_OPTION</a> for
                    a list of flags. If out message is not available, or no flags are needed, this may be 0.
                


<a href="https://msdn.microsoft.com/3f54e012-4893-4f70-9f38-55ae9db365e8">WS_SERVICE_OPERATION_MESSAGE_NILLABLE_ELEMENT</a> is not applicable to <a href="https://msdn.microsoft.com/c0cc2c3c-5050-444a-95e9-2cfb0e755253">WS_RPC_LITERAL_OPERATION</a> style
                    operations. The output parameter must be with type of <a href="https://msdn.microsoft.com/c847940a-f97e-4605-a940-1d72de6a3695">WS_PARAMETER_TYPE_MESSAGES</a>.
                


### -field parameterCount

The number of  parameters on the given service operation.
                


### -field parameterDescription

An array defining the individual parameters.
                


### -field stubCallback

A pointer to the stub function for the given operation to which the service model will delegate 
                    to do the service operation call. This will be <b>NULL</b> for proxies. 
                


### -field style

 



