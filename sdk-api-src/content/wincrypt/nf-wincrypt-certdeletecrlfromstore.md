---
UID: NF:wincrypt.CertDeleteCRLFromStore
title: CertDeleteCRLFromStore function
author: windows-sdk-content
description: The CertDeleteCRLFromStore function deletes the specified certificate revocation list (CRL) context from the certificate store.
old-location: security\certdeletecrlfromstore.htm
tech.root: SecCrypto
ms.assetid: eb542c25-8d2b-4427-8f2a-719b472613a5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CertDeleteCRLFromStore, CertDeleteCRLFromStore function [Security], _crypto2_certdeletecrlfromstore, security.certdeletecrlfromstore, wincrypt/CertDeleteCRLFromStore
ms.topic: function
req.header: wincrypt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
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
 - CertDeleteCRLFromStore
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CertDeleteCRLFromStore function


## -description


The <b>CertDeleteCRLFromStore</b> function deletes the specified <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate revocation list</a> (CRL) context from the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate store</a>.


## -parameters




### -param pCrlContext [in]

A pointer to the 
<a href="https://msdn.microsoft.com/cf7cabcd-b469-492a-b855-8870465ea1cc">CRL_CONTEXT</a> structure to be deleted.


## -returns



If the function succeeds, the return value is <b>TRUE</b>.

If the function fails, the return value is <b>FALSE</b>. For extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. One possible error code is the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_ACCESSDENIED</b></dt>
</dl>
</td>
<td width="60%">
The store was opened read-only, and a delete operation is not allowed.

</td>
</tr>
</table>
 




## -remarks



All subsequent get or find operations for the CRL in this store fail. However, memory allocated for the CRL is not freed until all duplicated contexts have also been freed.

The <i>pCrlContext</i> parameter is always freed by this function by using 
<a href="https://msdn.microsoft.com/19a590a5-bd39-4bbe-ad86-4e648baa1ba8">CertFreeCRLContext</a>, even for an error.




## -see-also




<a href="https://msdn.microsoft.com/19a590a5-bd39-4bbe-ad86-4e648baa1ba8">CertFreeCRLContext</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa380252(v=VS.85).aspx">Certificate Revocation List Functions</a>
 

 

