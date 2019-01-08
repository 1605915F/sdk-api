---
UID: NF:certpoleng.PstValidate
title: PstValidate function
author: windows-sdk-content
description: Validates the specified certificate.
old-location: security\pstvalidate.htm
tech.root: SecAuthN
ms.assetid: 4e1c4ebd-977e-4967-8ff6-694be0016276
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PstValidate, PstValidate function [Security], certpoleng/PstValidate, security.pstvalidate
ms.topic: function
req.header: certpoleng.h
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
req.lib: Certpoleng.lib
req.dll: Certpoleng.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Certpoleng.dll
api_name:
 - PstValidate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PstValidate function


## -description


Validates the specified certificate.


## -parameters




### -param pTargetName [in, optional]

The name of the server. If the caller is not the client, this parameter is <b>NULL</b>.


### -param bIsClient [in]

<b>TRUE</b> if the caller is the client; otherwise, <b>FALSE</b>.


### -param pRequestedIssuancePolicy [in, optional]

A pointer to a <a href="https://msdn.microsoft.com/6154f1f7-4293-4b8e-91ab-9f57bb6f5743">CERT_USAGE_MATCH</a> structure that specifies identifiers that the certificate must match to be validated.


### -param phAdditionalCertStore [in, optional]

A handle to a <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate store</a> that contains additional certificates used for the authentication.


### -param pCert [in]

A pointer to a <a href="https://msdn.microsoft.com/f0a3200e-6541-423d-a4a3-595a31026eea">CERT_CONTEXT</a> structure that specifies the certificate to validate.


### -param pProvGUID [out, optional]

A pointer to  a <b>GUID</b> structure that receives the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security support provider</a> (SSP) used for the authentication.


## -returns



If the function succeeds, return <b>STATUS_SUCCESS</b>.

If the function fails, return an <b>NTSTATUS</b> code that indicates the reason it failed.



