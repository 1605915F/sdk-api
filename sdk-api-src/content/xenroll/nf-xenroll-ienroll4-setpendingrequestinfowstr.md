---
UID: NF:xenroll.IEnroll4.setPendingRequestInfoWStr
title: IEnroll4::setPendingRequestInfoWStr (xenroll.h)
author: windows-sdk-content
description: Sets properties for a pending request.
old-location: security\ienroll4_setpendingrequestinfowstr.htm
tech.root: SecCrypto
ms.assetid: 02b49033-3354-4e30-a816-a9c078c6164a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IEnroll4 interface [Security],setPendingRequestInfoWStr method, IEnroll4.setPendingRequestInfoWStr, IEnroll4::setPendingRequestInfoWStr, security.ienroll4_setpendingrequestinfowstr, setPendingRequestInfoWStr, setPendingRequestInfoWStr method [Security], setPendingRequestInfoWStr method [Security],IEnroll4 interface, xenroll/IEnroll4::setPendingRequestInfoWStr
ms.topic: method
req.header: xenroll.h
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
req.lib: Uuid.lib
req.dll: Xenroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Xenroll.dll
api_name:
 - IEnroll4.setPendingRequestInfoWStr
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IEnroll4::setPendingRequestInfoWStr


## -description


<p class="CCE_Message">[This method is no longer available for use as of Windows Server 2008 and Windows Vista.]

The <b>setPendingRequestInfoWStr</b> method sets properties for a pending request. This method was first defined in the <a href="https://msdn.microsoft.com/133529fb-e02a-41a2-83df-646cbc01dbe9">IEnroll4</a> interface.


## -parameters




### -param lRequestID [in]

Identifier for the request, as assigned by the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certification authority</a> (CA).


### -param pwszCADNS [in]

A pointer to a null-terminated wide character string that represents the CA's Domain Name System (DNS) name. This parameter cannot be null.


### -param pwszCAName [in]

A pointer to a null-terminated wide character string that represents the CA's name. This parameter cannot be null.


### -param pwszFriendlyName [in]

A pointer to a null-terminated wide character string that represents the CA's display name. This parameter may be null.


## -see-also




<a href="https://msdn.microsoft.com/133529fb-e02a-41a2-83df-646cbc01dbe9">IEnroll4</a>
 

 

