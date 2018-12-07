---
UID: NF:certenc.ICertEncodeBitString.GetBitString
title: ICertEncodeBitString::GetBitString
author: windows-sdk-content
description: Returns the string of bits in the object's bit string.
old-location: security\icertencodebitstring_getbitstring.htm
tech.root: seccrypto
ms.assetid: d0c6c501-3aaa-42ab-a077-69f6d24f1eff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CCertEncodeBitString object [Security],GetBitString method, GetBitString, GetBitString method [Security], GetBitString method [Security],CCertEncodeBitString object, GetBitString method [Security],ICertEncodeBitString interface, ICertEncodeBitString interface [Security],GetBitString method, ICertEncodeBitString.GetBitString, ICertEncodeBitString::GetBitString, _certsrv_icertencodebitstring_getbitstring, certenc/ICertEncodeBitString::GetBitString, security.icertencodebitstring_getbitstring
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenc.h
req.include-header: Certsrv.h
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.lib: Certidl.lib
req.dll: Certenc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certenc.dll
api_name:
 - ICertEncodeBitString.GetBitString
 - CCertEncodeBitString.GetBitString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertEncodeBitString::GetBitString


## -description


The <b>GetBitString</b> method returns the string of bits in the object's bit string.


## -parameters




### -param pstrBitString [out]

A pointer to a <b>BSTR</b> that will contain the bit string. When you have finished using the <b>BSTR</b>, free it by calling the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<h3>VB</h3>
 The return value is the bit string.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa383767(v=VS.85).aspx">ICertEncodeBitString</a>
 

 

