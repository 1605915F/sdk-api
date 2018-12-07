---
UID: NF:certenroll.IX509SCEPEnrollment.get_Request
title: IX509SCEPEnrollment::get_Request
author: windows-sdk-content
description: Gets the inner PKCS10 request.
old-location: security\ix509scepenrollment_request.htm
tech.root: seccertenroll
ms.assetid: 9446cd62-5a02-4701-8b13-9e46508fbfaa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IX509SCEPEnrollment interface [Security],Request property, IX509SCEPEnrollment.Request, IX509SCEPEnrollment.get_Request, IX509SCEPEnrollment::Request, IX509SCEPEnrollment::get_Request, Request property [Security], Request property [Security],IX509SCEPEnrollment interface, certenroll/IX509SCEPEnrollment::Request, certenroll/IX509SCEPEnrollment::get_Request, get_Request, security.ix509scepenrollment_request
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
 - IX509SCEPEnrollment.Request
 - IX509SCEPEnrollment.get_Request
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509SCEPEnrollment::get_Request


## -description


Gets the inner PKCS10 request.

This property is read-only.


## -parameters


## -remarks



You can use the inner PKCS10 request instance to set the subject, extensions, private key properties, encryption algorithm and strength, and the hash algorithm before you call the <a href="https://msdn.microsoft.com/en-us/library/Dn424976(v=VS.85).aspx">CreateRequestMessage</a> method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn424973(v=VS.85).aspx">IX509SCEPEnrollment</a>
 

 

