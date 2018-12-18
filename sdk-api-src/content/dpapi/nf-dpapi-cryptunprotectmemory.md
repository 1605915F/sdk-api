---
UID: NF:dpapi.CryptUnprotectMemory
title: CryptUnprotectMemory function
author: windows-sdk-content
description: Decrypts memory that was encrypted using the CryptProtectMemory function.
old-location: security\cryptunprotectmemory.htm
tech.root: seccrypto
ms.assetid: 1c7980ac-4e9e-43fd-b6d7-c0d0a69c8040
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CRYPTPROTECTMEMORY_CROSS_PROCESS, CRYPTPROTECTMEMORY_SAME_LOGON, CRYPTPROTECTMEMORY_SAME_PROCESS, CryptUnprotectMemory, CryptUnprotectMemory function [Security], dpapi/CryptUnprotectMemory, security.cryptunprotectmemory, wincrypt/CryptUnprotectMemory
ms.topic: function
req.header: dpapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
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
 - CryptUnprotectMemory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CryptUnprotectMemory function


## -description


The <b>CryptUnprotectMemory</b> function decrypts memory that was encrypted using the <a href="https://msdn.microsoft.com/6b372552-87d4-4047-afa5-0d1113348289">CryptProtectMemory</a> function.


## -parameters




### -param pDataIn [in, out]

A pointer to the block of memory to decrypt. The <i>cbData</i> parameter specifies the number of bytes that the function will attempt to decrypt. If the data contained in the memory space is smaller than the number of bytes specified, the function will attempt to decrypt data outside of the intended block. If it is larger than <i>cbData</i> bytes, then only the first <i>cbData</i> bytes will be decrypted.


### -param cbDataIn [in]

Number of bytes of memory pointed to by the <i>pData</i> parameter to decrypt. The number of bytes must be a multiple of the <b>CRYPTPROTECTMEMORY_BLOCK_SIZE</b> constant defined in Wincrypt.h.


### -param dwFlags [in]

This parameter can be one of the following flags. You must specify the same flag when encrypting and decrypting the memory.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="CRYPTPROTECTMEMORY_SAME_PROCESS"></a><a id="cryptprotectmemory_same_process"></a><dl>
<dt><b>CRYPTPROTECTMEMORY_SAME_PROCESS</b></dt>
</dl>
</td>
<td width="60%">
Encrypt and decrypt memory in the same process. An application running in a different process will not be able to decrypt the data.

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPTPROTECTMEMORY_CROSS_PROCESS"></a><a id="cryptprotectmemory_cross_process"></a><dl>
<dt><b>CRYPTPROTECTMEMORY_CROSS_PROCESS</b></dt>
</dl>
</td>
<td width="60%">
Encrypt and decrypt memory in different processes. An application running in a different process will be able to decrypt the data.

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPTPROTECTMEMORY_SAME_LOGON"></a><a id="cryptprotectmemory_same_logon"></a><dl>
<dt><b>CRYPTPROTECTMEMORY_SAME_LOGON</b></dt>
</dl>
</td>
<td width="60%">
Use the same logon credentials to encrypt and decrypt memory in different processes. An application running in a different process will be able to decrypt the data. However, the process must run as the same user that encrypted the data and in the same logon session.

</td>
</tr>
</table>
 


## -returns



If the function succeeds, the function returns <b>TRUE</b>.

If the function fails, it returns <b>FALSE</b>. For extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



Using  <a href="https://msdn.microsoft.com/en-us/library/Aa380262(v=VS.85).aspx">CryptProtectMemory</a> and <a href="https://msdn.microsoft.com/en-us/library/Aa380890(v=VS.85).aspx">CryptUnprotectMemory</a> for password encryption is not secure because the data exists as plaintext in memory before it is encrypted and at any time the caller decrypts it for use.

 You must encrypt and decrypt the memory during the same boot session. If the computer is restarted before you call the <b>CryptUnprotectMemory</b> function, you will not be able to decrypt the data.

You must pass the same flag to <b>CryptUnprotectMemory</b> and <a href="https://msdn.microsoft.com/6b372552-87d4-4047-afa5-0d1113348289">CryptProtectMemory</a>. If you pass different flags, the <b>CryptUnprotectMemory</b> function succeeds; however, the result is unpredictable.

 When you have finished using the sensitive information, clear it from memory by calling the <a href="https://msdn.microsoft.com/2c4090a6-025b-4b7b-8f31-7e744ad51b39">SecureZeroMemory</a> function.


#### Examples

The following example calls  the <b>CryptUnprotectMemory</b> function to decrypt data that is in memory. The example assumes the variable pEncryptedText points to a string that has been encrypted using the <a href="https://msdn.microsoft.com/6b372552-87d4-4047-afa5-0d1113348289">CryptProtectMemory</a> function.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#include &lt;windows.h&gt;
#include &lt;stdio.h&gt;
#include &lt;Wincrypt.h&gt;
#include &lt;strsafe.h&gt;
#pragma comment(lib, "crypt32.lib")

void main()
{
    LPWSTR pEncryptedText;  // contains the encrypted text
    DWORD cbEncryptedText;  // number of bytes to which 
	                        // pEncryptedText points

    if (CryptUnprotectMemory(pEncryptedText, cbEncryptedText, 
		CRYPTPROTECTMEMORY_SAME_PROCESS))
    {
        // Use the decrypted string.
    }
    else
    {
        wprintf(L"CryptUnprotectMemory failed: %d\n", 
			GetLastError());
    }

    // Clear and free memory after using
    // the decrypted string or if an error occurs. 
    SecureZeroMemory(pEncryptedText, cbEncryptedText);
    LocalFree(pEncryptedText);
    pEncryptedText = NULL;
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/6b372552-87d4-4047-afa5-0d1113348289">CryptProtectMemory</a>



<a href="https://msdn.microsoft.com/54eab3b0-d341-47c6-9c32-79328d7a7155">CryptUnprotectData</a>



<a href="https://msdn.microsoft.com/8ecc5007-92ce-4e32-a093-dcb75ee8ba62">RtlDecryptMemory</a>



<a href="https://msdn.microsoft.com/b124a7fe-c62c-42f7-9d2b-cbf74d17186a">RtlEncryptMemory</a>
 

 

