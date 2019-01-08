---
UID: NS:wincrypt._CRL_ISSUING_DIST_POINT
title: CRL_ISSUING_DIST_POINT
author: windows-sdk-content
description: Contains information about the kinds of certificates listed in a certificate revocation list (CRL).
old-location: security\crl_issuing_dist_point.htm
tech.root: SecCrypto
ms.assetid: cdac9e96-5b26-4398-8863-16ea2c43f11e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCRL_ISSUING_DIST_POINT, CRL_ISSUING_DIST_POINT, CRL_ISSUING_DIST_POINT structure [Security], PCRL_ISSUING_DIST_POINT, PCRL_ISSUING_DIST_POINT structure pointer [Security], _crypto2_crl_issuing_dist_point, security.crl_issuing_dist_point, wincrypt/CRL_ISSUING_DIST_POINT, wincrypt/PCRL_ISSUING_DIST_POINT"
ms.topic: struct
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
 - HeaderDef
api_location:
 - Wincrypt.h
api_name:
 - CRL_ISSUING_DIST_POINT
product: Windows
targetos: Windows
req.typenames: CRL_ISSUING_DIST_POINT, *PCRL_ISSUING_DIST_POINT
req.redist: 
---

# CRL_ISSUING_DIST_POINT structure


## -description


The <b>CRL_ISSUING_DIST_POINT</b> structure contains information about the kinds of certificates listed in a <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate revocation list</a> (CRL).


## -struct-fields




### -field DistPointName

Optional 
<a href="https://msdn.microsoft.com/f47283c3-34f5-4611-b041-456d28d85dbe">CRL_DIST_POINT_NAME</a> member.


### -field fOnlyContainsUserCerts

<b>BOOL</b> flag. <b>TRUE</b> if only user certificates are contained in the CRL.


### -field fOnlyContainsCACerts

<b>BOOL</b> flag. <b>TRUE</b> if only CA certificates are contained in the CRL.


### -field OnlySomeReasonFlags

Optional 
<a href="https://msdn.microsoft.com/6f102ff3-bfff-4415-a5d8-ca2c226074b3">CRYPT_BIT_BLOB</a> with bits indicating some reasons for certificate revocation.


### -field fIndirectCRL

<b>BOOL</b> flag. <b>TRUE</b> if this is an indirect CRL.

