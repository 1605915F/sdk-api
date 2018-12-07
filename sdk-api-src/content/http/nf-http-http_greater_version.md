---
UID: NF:http.HTTP_GREATER_VERSION
title: HTTP_GREATER_VERSION macro
author: windows-sdk-content
description: Returns a non-zero value if an HTTP_VERSION structure is greater than a specified major/minor version combination, or zero otherwise.
old-location: http\http_greater_version.htm
tech.root: http
ms.assetid: 741b6f26-4c87-459e-a672-daf098f0c9e6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HTTP_GREATER_VERSION, HTTP_GREATER_VERSION macro [HTTP], _http_http_greater_version, http.http_greater_version, http/HTTP_GREATER_VERSION
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: macro
req.header: http.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
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
 - Http.h
api_name:
 - HTTP_GREATER_VERSION
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# HTTP_GREATER_VERSION macro


## -description


The 
<b>HTTP_GREATER_VERSION</b> macro returns a non-zero value if an 
<a href="https://msdn.microsoft.com/8f97410c-27b5-4225-849e-ee55e4c5f762">HTTP_VERSION</a> structure is greater than a specified major/minor version combination, or zero otherwise.


## -parameters




### -param version

The 
<a href="https://msdn.microsoft.com/8f97410c-27b5-4225-849e-ee55e4c5f762">HTTP_VERSION</a> structure to be examined.


### -param major

The major portion of the version to be compared.


### -param minor

The minor portion of the version to be compared.


## -see-also




<a href="https://msdn.microsoft.com/9c5fb0a4-fda8-4489-8a1e-c232079bd501">HTTP Server API Version 1.0 Macros</a>
 

 

