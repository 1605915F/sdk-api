---
UID: NC:wincrypt.PFN_CERT_STORE_PROV_WRITE_CTL
title: PFN_CERT_STORE_PROV_WRITE_CTL
author: windows-sdk-content
description: The CertStoreProvWriteCTL callback function can be called by CertAddEncodedCTLToStore, CertAddCTLContextToStore or CertAddSerializedElementToStore before a CTL is added to the store.
old-location: security\certstoreprovwritectl.htm
tech.root: seccrypto
ms.assetid: 91344133-0785-4c4f-8df3-83301cf85e70
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CertStoreProvWriteCTL, PFN_CERT_STORE_PROV_WRITE_CTL, PFN_CERT_STORE_PROV_WRITE_CTL callback, PFN_CERT_STORE_PROV_WRITE_CTL callback function [Security], _crypto2_certstoreprovwritectl, security.certstoreprovwritectl, wincrypt/PFN_CERT_STORE_PROV_WRITE_CTL
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - PFN_CERT_STORE_PROV_WRITE_CTL
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFN_CERT_STORE_PROV_WRITE_CTL callback function


## -description


The <b>CertStoreProvWriteCTL</b> callback function can be called by 
<a href="https://msdn.microsoft.com/4239d43e-187d-4f40-99ae-6f914b7577ac">CertAddEncodedCTLToStore</a>, 
<a href="https://msdn.microsoft.com/e8858f75-77a1-4c5f-a3e3-a645c5e0f053">CertAddCTLContextToStore</a> or 
<a href="https://msdn.microsoft.com/2726cd34-51ba-4f68-9a3c-7cd505eb32a1">CertAddSerializedElementToStore</a> before a CTL is added to the store.


## -parameters




### -param hStoreProv [in]

<b>HCERTSTOREPROV</b> handle to a <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate store</a>.


### -param pCtlContext [in]

A pointer to a 
<a href="https://msdn.microsoft.com/780edddf-1b44-4292-9156-4dfd5100adb8">CTL_CONTEXT</a> structure.


### -param dwFlags [in]

Any needed flag values.


## -returns



Returns <b>TRUE</b> if elements can be added to the store.




## -see-also




<a href="https://msdn.microsoft.com/780edddf-1b44-4292-9156-4dfd5100adb8">CTL_CONTEXT</a>



<a href="https://msdn.microsoft.com/e8858f75-77a1-4c5f-a3e3-a645c5e0f053">CertAddCTLContextToStore</a>



<a href="https://msdn.microsoft.com/4239d43e-187d-4f40-99ae-6f914b7577ac">CertAddEncodedCTLToStore</a>



<a href="https://msdn.microsoft.com/2726cd34-51ba-4f68-9a3c-7cd505eb32a1">CertAddSerializedElementToStore</a>
 

 

