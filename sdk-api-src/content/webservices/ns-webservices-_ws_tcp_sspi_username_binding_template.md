---
UID: NS:webservices._WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE
title: "_WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE"
author: windows-sdk-content
description: Username/password security template information to be filled in by application. Associated with WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE_TYPE.
old-location: wsw\ws_tcp_sspi_username_binding_template.htm
tech.root: wsw
ms.assetid: c2d63721-0810-48a5-b1f8-8b1adcba96b8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE, WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE structure [Web Services for Windows], _WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE, webservices/WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE, wsw.ws_tcp_sspi_username_binding_template
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE
product: Windows
targetos: Windows
req.typenames: WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE
req.redist: 
---

# _WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE structure


## -description


Username/password security template information to be filled in by application.
        Associated with <a href="https://msdn.microsoft.com/831001f4-619d-4128-a645-85077701c28c">WS_TCP_SSPI_USERNAME_BINDING_TEMPLATE_TYPE</a>.
      


## -struct-fields




### -field channelProperties

Application provided additional channel properties that cannot be represented in policy.
        


### -field securityProperties

Application provided additional security properties that cannot be represented in policy.
        


### -field sspiTransportSecurityBinding

Application provided SSPI transport security information that cannot be represented
          in policy.
        


### -field usernameMessageSecurityBinding

Application provided username/password authentication binding information
          that cannot be represented in policy.
        

