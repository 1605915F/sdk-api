---
UID: NS:bits1_5.__MIDL_IBackgroundCopyJob2_0005
title: BG_AUTH_CREDENTIALS (bits1_5.h)
author: windows-sdk-content
description: Identifies the target (proxy or server), authentication scheme, and the user's credentials to use for user authentication requests. The structure is passed to the IBackgroundCopyJob2::SetCredentials method.
old-location: bits\bg_auth_credentials.htm
tech.root: Bits
ms.assetid: f89ebf46-da83-495c-bafe-b2e0f72f5d8e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PBG_AUTH_CREDENTIALS, BG_AUTH_CREDENTIALS, BG_AUTH_CREDENTIALS structure [BITS], _drz_bg_auth_credentials, bits.bg_auth_credentials, bits1_5/BG_AUTH_CREDENTIALS"
ms.topic: struct
req.header: bits1_5.h
req.include-header: Bits.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2003
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits1_5.idl
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
 - Bits1_5.h
api_name:
 - BG_AUTH_CREDENTIALS
product: Windows
targetos: Windows
req.typenames: BG_AUTH_CREDENTIALS
req.redist: BITS 1.5 on  Windows XP
ms.custom: 19H1
---

# BG_AUTH_CREDENTIALS structure


## -description

Identifies the target (proxy or server), authentication scheme, and the user's credentials to use for user authentication requests. The structure is passed to the 
<a href="https://msdn.microsoft.com/adaffc21-7df1-48ca-8e05-bdb09663a49b">IBackgroundCopyJob2::SetCredentials</a> method.


## -struct-fields




### -field Target

Identifies whether to use the credentials for a proxy or server authentication request. For a list of values, see the 
<a href="https://msdn.microsoft.com/efe7aa0a-48fc-4192-b81b-40d3a9b0fb22">BG_AUTH_TARGET</a> enumeration. You can specify only one value.


### -field Scheme

Identifies the scheme to use for authentication (for example, Basic or NTLM). For a list of values, see the 
<a href="https://msdn.microsoft.com/e5a97cee-0012-4e30-850a-9adc258a36d3">BG_AUTH_SCHEME</a> enumeration. You can specify only one value.


### -field Credentials

Identifies the credentials to use for the specified authentication scheme. For details, see the 
<a href="https://msdn.microsoft.com/c16c616c-f4cb-483d-8a15-6ff9d45762ae">BG_AUTH_CREDENTIALS_UNION</a> union.


## -see-also




<a href="https://msdn.microsoft.com/c16c616c-f4cb-483d-8a15-6ff9d45762ae">BG_AUTH_CREDENTIALS_UNION</a>



<a href="https://msdn.microsoft.com/e5a97cee-0012-4e30-850a-9adc258a36d3">BG_AUTH_SCHEME</a>



<a href="https://msdn.microsoft.com/efe7aa0a-48fc-4192-b81b-40d3a9b0fb22">BG_AUTH_TARGET</a>



<a href="https://msdn.microsoft.com/adaffc21-7df1-48ca-8e05-bdb09663a49b">IBackgroundCopyJob2::SetCredentials</a>
 

 

