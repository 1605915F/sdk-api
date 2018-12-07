---
UID: NF:certenroll.IX509SCEPEnrollment.CreateRetrieveCertificateMessage
title: IX509SCEPEnrollment::CreateRetrieveCertificateMessage
author: windows-sdk-content
description: Retrieve a previously issued certificate.
old-location: security\ix509scepenrollment_createretrievecertificatemessage.htm
tech.root: seccertenroll
ms.assetid: 238a837f-4464-49ce-b87a-03abcfc0abea
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateRetrieveCertificateMessage, CreateRetrieveCertificateMessage method [Security], CreateRetrieveCertificateMessage method [Security],IX509SCEPEnrollment interface, IX509SCEPEnrollment interface [Security],CreateRetrieveCertificateMessage method, IX509SCEPEnrollment.CreateRetrieveCertificateMessage, IX509SCEPEnrollment::CreateRetrieveCertificateMessage, certenroll/IX509SCEPEnrollment::CreateRetrieveCertificateMessage, security.ix509scepenrollment_createretrievecertificatemessage
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certenroll.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Certenroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certenroll.dll
api_name:
 - IX509SCEPEnrollment.CreateRetrieveCertificateMessage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509SCEPEnrollment::CreateRetrieveCertificateMessage


## -description


Retrieve a previously issued certificate.


## -parameters




### -param Context [in]


### -param strIssuer [in]

ASN.1 encoded issuer name.


### -param IssuerEncoding [in]


### -param strSerialNumber [in]


### -param SerialNumberEncoding [in]


### -param Encoding [in]


### -param pValue [out, retval]


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



You must call the <a href="https://msdn.microsoft.com/en-us/library/Dn424982(v=VS.85).aspx">InitializeForPending</a> method before calling this method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn424973(v=VS.85).aspx">IX509SCEPEnrollment</a>
 

 

