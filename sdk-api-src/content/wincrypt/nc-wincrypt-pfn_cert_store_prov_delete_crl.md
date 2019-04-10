---
UID: NC:wincrypt.PFN_CERT_STORE_PROV_DELETE_CRL
title: PFN_CERT_STORE_PROV_DELETE_CRL (wincrypt.h)
author: windows-sdk-content
description: An application-defined callback function that is called by CertDeleteCRLFromStore before deleting the CRL from the store.
old-location: security\certstoreprovdeletecrlcallback.htm
tech.root: SecCrypto
ms.assetid: aa93cfaf-238f-4d77-a1cd-433a856ed133
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CertStoreProvDeleteCRLCallback, PFN_CERT_STORE_PROV_DELETE_CRL, PFN_CERT_STORE_PROV_DELETE_CRL callback, PFN_CERT_STORE_PROV_DELETE_CRL callback function [Security], _crypto2_certstoreprovdeletecrlcallback, security.certstoreprovdeletecrlcallback, wincrypt/PFN_CERT_STORE_PROV_DELETE_CRL
ms.topic: callback
req.header: wincrypt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - UserDefined
api_location:
 - Wincrypt.h
api_name:
 - PFN_CERT_STORE_PROV_DELETE_CRL
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFN_CERT_STORE_PROV_DELETE_CRL callback function


## -description


An application-defined callback function that is called by 
<a href="https://msdn.microsoft.com/eb542c25-8d2b-4427-8f2a-719b472613a5">CertDeleteCRLFromStore</a> before deleting the CRL from the store.


## -parameters




### -param hStoreProv [in]

Provider-specific value returned in 
<a href="https://msdn.microsoft.com/dc6789a7-09a5-467a-b2e4-16acfa25b5f6">CERT_STORE_PROV_INFO</a> by 
<a href="https://msdn.microsoft.com/2fe291dd-23e2-49df-b9e4-a4ed29667123">CertDllOpenStoreProv</a>.


### -param pCrlContext [in]

A pointer to the CRL context to be deleted.


### -param dwFlags [in]

Reserved for future use and is set to zero.


## -returns



Returns <b>TRUE</b> if it is okay to delete from the store. Otherwise, returns <b>FALSE</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa380252(v=VS.85).aspx">Callback Functions</a>
 

 

