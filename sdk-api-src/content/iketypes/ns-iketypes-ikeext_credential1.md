---
UID: NS:iketypes.IKEEXT_CREDENTIAL1_
title: IKEEXT_CREDENTIAL1
author: windows-sdk-content
description: Is used to store credential information used for the authentication.
old-location: fwp\ikeext_credential1.htm
tech.root: fwp
ms.assetid: 81b4c66a-67dd-4d5a-bd71-2fdbe6fd5df5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IKEEXT_CREDENTIAL1, IKEEXT_CREDENTIAL1 structure [Filtering], fwp.ikeext_credential1, iketypes/IKEEXT_CREDENTIALS1
ms.topic: struct
req.header: iketypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Iketypes.idl
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
 - Iketypes.h
api_name:
 - IKEEXT_CREDENTIAL1
product: Windows
targetos: Windows
req.typenames: IKEEXT_CREDENTIAL1
req.redist: 
---

# IKEEXT_CREDENTIAL1 structure


## -description


The <b>IKEEXT_CREDENTIAL1</b> structure is  used to store credential information used for the authentication.
<div class="alert"><b>Note</b>  <b>IKEEXT_CREDENTIAL1</b> is the specific implementation of IKEEXT_CREDENTIAL used in Windows 7. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 8, <a href="https://msdn.microsoft.com/b27689ef-5e2a-4163-a4d7-40f8939d4c66">IKEEXT_CREDENTIAL2</a> is available. For Windows Vista, <a href="https://msdn.microsoft.com/cb5aa4b6-71e7-43d4-a69c-4f209cd9755b">IKEEXT_CREDENTIAL0</a> is available.</div><div> </div>

## -struct-fields




### -field authenticationMethodType

Type of authentication method.

See <a href="https://msdn.microsoft.com/en-us/library/Aa364977(v=VS.85).aspx">IKEEXT_AUTHENTICATION_METHOD_TYPE</a> for more information.


### -field impersonationType

Type of impersonation.

See <a href="https://msdn.microsoft.com/en-us/library/Aa364974(v=VS.85).aspx">IKEEXT_AUTHENTICATION_IMPERSONATION_TYPE</a> for more information.


### -field presharedKey

Available when <b>authenticationMethodType</b> is <b>IKEEXT_PRESHARED_KEY</b>.

See <a href="https://msdn.microsoft.com/en-us/library/Dd744976(v=VS.85).aspx">IKEEXT_PRESHARED_KEY_AUTHENTICATION1</a> for more information.


### -field certificate

Available when <b>authenticationMethodType</b> is one of the following values.

<b>IKEEXT_CERTIFICATE</b>
<b>IKEEXT_CERTIFICATE_ECDSA_P256</b>
<b>IKEEXT_CERTIFICATE_ECDSA_P384</b>
<b>IKEEXT_SSL</b>
<b>IKEEXT_SSL_ECDSA_P256</b>
<b>IKEEXT_SSL_ECDSA_P384</b>
<b>IKEEXT_IPV6_CGA</b>
See <a href="https://msdn.microsoft.com/78ae9cfe-2a4f-48cd-9a4f-fd5193df0ed0">IKEEXT_CERTIFICATE_CREDENTIAL1</a> for more information.


### -field name

Available when <b>authenticationMethodType</b> is one of the following values.

<b>IKEEXT_KERBEROS</b>
<b>IKEEXT_NTML_V2</b>
See <a href="https://msdn.microsoft.com/602f94bf-066d-418e-a469-a21b881a443d">IKEEXT_NAME_CREDENTIAL0</a> for more information.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa364974(v=VS.85).aspx">IKEEXT_AUTHENTICATION_IMPERSONATION_TYPE</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa364977(v=VS.85).aspx">IKEEXT_AUTHENTICATION_METHOD_TYPE</a>



<a href="https://msdn.microsoft.com/78ae9cfe-2a4f-48cd-9a4f-fd5193df0ed0">IKEEXT_CERTIFICATE_CREDENTIAL1</a>



<a href="https://msdn.microsoft.com/602f94bf-066d-418e-a469-a21b881a443d">IKEEXT_NAME_CREDENTIAL0</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd744976(v=VS.85).aspx">IKEEXT_PRESHARED_KEY_AUTHENTICATION1</a>



<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 

