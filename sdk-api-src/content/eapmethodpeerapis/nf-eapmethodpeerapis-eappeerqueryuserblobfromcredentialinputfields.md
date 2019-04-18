---
UID: NF:eapmethodpeerapis.EapPeerQueryUserBlobFromCredentialInputFields
title: EapPeerQueryUserBlobFromCredentialInputFields function (eapmethodpeerapis.h)
author: windows-sdk-content
description: Defines the implementation of an EAP method function that obtains the user BLOB data provided in an interactive Single-Sign-On (SSO) UI raised on the supplicant.
old-location: eaphost\eappeerqueryuserblobfrominteractiveuiinputfields.htm
tech.root: eaphost
ms.assetid: decfe3cd-642e-41c8-9bec-d079a0f74504
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EapPeerQueryUserBlobFromCredentialInputFields, EapPeerQueryUserBlobFromCredentialInputFields function [EAPHost], eaphost.eappeerqueryuserblobfrominteractiveuiinputfields, eapmethodpeerapis/EapPeerQueryUserBlobFromCredentialInputFields
ms.topic: function
req.header: eapmethodpeerapis.h
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
 - eapmethodpeerapis.h
api_name:
 - EapPeerQueryUserBlobFromCredentialInputFields
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# EapPeerQueryUserBlobFromCredentialInputFields function


## -description


The <b>EapPeerQueryUserBlobFromCredentialInputFields</b> function defines the implementation of an EAP method function that obtains the user BLOB data provided in an interactive Single-Sign-On (SSO) UI raised on the supplicant.


## -parameters




### -param hUserImpersonationToken [in]

An impersonation token for the user whose credentials are to be requested and obtained. 


### -param eapMethodType [in]

An <a href="https://msdn.microsoft.com/47702dd9-d9c2-4dd5-a12d-23a55b031d27">EAP_METHOD_TYPE</a> structure that contains vendor and author information about the EAP method used for authenticating the connection.


### -param dwFlags [in]

A combination of <a href="https://msdn.microsoft.com/b6305349-3418-475e-8a37-2c06b399556e">EAP flags</a> that describe the  EAP authentication session behavior.


### -param dwEapConnDataSize [in]

The size of the EAP SSO configuration  data pointed to by <i>pbEapConnData</i>, in bytes. 



### -param pbEapConnData [in]

A pointer to an opaque byte buffer that contains the EAP SSO configuration data BLOB. 


### -param pEapConfigInputFieldArray [in]

A pointer to an <a href="https://msdn.microsoft.com/e8a2e934-1ded-4159-8cd8-7aeb75ce743a">EAP_CONFIG_INPUT_FIELD_ARRAY</a> structure that contains the input fields to display to the supplicant user. The <b>pwszData</b> fields in the individual <a href="https://msdn.microsoft.com/2b321f26-fb40-44e5-b483-52d85cb54c8c">EAP_CONFIG_INPUT_FIELD_DATA</a> elements are initialized to <b>NULL</b>.


### -param pdwUserBlobSize [in, out]

A pointer to a buffer that contains the size, in bytes, of the opaque user configuration data BLOB in <i>ppUserBlob</i>.


### -param ppbUserBlob [in, out]

A pointer that contains the opaque user data BLOB. 



### -param ppEapError [out]

 A pointer to the address of an <a href="https://msdn.microsoft.com/6af8cb67-da77-491a-98de-df10b6b7f46d">EAP_ERROR</a> structure that contains any errors raised during  the execution of this function call. After consuming the error data, this memory must be freed by passing a pointer to the error data to <a href="https://msdn.microsoft.com/85b4197c-5caf-4e2b-94fd-e651712dd39d">EapPeerFreeErrorMemory</a>.


## -remarks



<b>EapPeerQueryUserBlobFromCredentialInputFields</b> supports Single-Sign-On (SSO). This peer method function, like <a href="https://msdn.microsoft.com/8ae42352-e972-4094-bf03-90a2f20ab641">EapPeerQueryCredentialInputFields</a>, is used only in an SSO scenario.

After <b>EapPeerQueryUserBlobFromCredentialInputFields</b>, EAPHost calls <a href="https://msdn.microsoft.com/770a548c-c227-4708-bc40-08bf2681c90f">EapPeerBeginSession</a>. The supplicant  uses the <b>EAP_FLAG_PRE_LOGON</b> flag in <b>EapHostPeerBeginSession</b> to indicate that EAPHost should provide SSO.




## -see-also




<a href="https://msdn.microsoft.com/e8a2e934-1ded-4159-8cd8-7aeb75ce743a">EAP_CONFIG_INPUT_FIELD_ARRAY</a>



<a href="https://msdn.microsoft.com/126ef6cc-aa65-4770-b81a-82d25213618c"> SSO and PLAP</a>
 

 

