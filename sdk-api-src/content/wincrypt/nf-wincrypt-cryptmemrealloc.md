---
UID: NF:wincrypt.CryptMemRealloc
title: CryptMemRealloc function (wincrypt.h)
author: windows-sdk-content
description: The CryptMemRealloc function frees the memory currently allocated for a buffer and allocates memory for a new buffer.
old-location: security\cryptmemrealloc.htm
tech.root: SecCrypto
ms.assetid: 74bdd2dd-9f05-4d36-8323-79d547820068
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CryptMemRealloc, CryptMemRealloc function [Security], _crypto2_cryptmemrealloc, security.cryptmemrealloc, wincrypt/CryptMemRealloc
ms.topic: function
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
req.lib: Crypt32.lib
req.dll: Crypt32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Crypt32.dll
api_name:
 - CryptMemRealloc
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CryptMemRealloc function


## -description


The <b>CryptMemRealloc</b> function frees the memory currently allocated for a buffer and allocates memory for a new buffer.


## -parameters




### -param pv [in]

A pointer to a currently allocated buffer.


### -param cbSize [in]

Number of bytes to be allocated.


## -returns



Returns a pointer to the buffer allocated. If the function fails, <b>NULL</b> is returned. When you have finished using the buffer, free the memory by calling the <a href="https://msdn.microsoft.com/fb5c10ba-da8e-4a34-9302-67586a0a9624">CryptMemFree</a> function.




## -see-also




<a href="https://msdn.microsoft.com/ac7588b1-ff8c-4f8d-a8ab-f0e8a18e5614">CryptMemAlloc</a>



<a href="https://msdn.microsoft.com/fb5c10ba-da8e-4a34-9302-67586a0a9624">CryptMemFree</a>
 

 

