---
UID: NF:certenc.ICertEncodeCRLDistInfo.Decode
title: ICertEncodeCRLDistInfo::Decode
author: windows-sdk-content
description: Decodes an Abstract Syntax Notation One (ASN.1)-encoded certificate revocation list (CRL) distribution information extension and stores the resulting array in the COM object.
old-location: security\icertencodecrldistinfo_decode.htm
tech.root: seccrypto
ms.assetid: 3df104a5-fbd7-4eb1-a6b2-b3e51afa15bf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CCertEncodeCRLDistInfo object [Security],Decode method, Decode, Decode method [Security], Decode method [Security],CCertEncodeCRLDistInfo object, Decode method [Security],ICertEncodeCRLDistInfo interface, ICertEncodeCRLDistInfo interface [Security],Decode method, ICertEncodeCRLDistInfo.Decode, ICertEncodeCRLDistInfo::Decode, _certsrv_icertencodecrldistinfo_decode, certenc/ICertEncodeCRLDistInfo::Decode, security.icertencodecrldistinfo_decode
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
 - ICertEncodeCRLDistInfo.Decode
 - CCertEncodeCRLDistInfo.Decode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertEncodeCRLDistInfo::Decode


## -description


The <b>Decode</b> method decodes an <a href="https://msdn.microsoft.com/en-us/library/ms721532(v=VS.85).aspx">Abstract Syntax Notation One</a> (ASN.1)-encoded <a href="https://msdn.microsoft.com/en-us/library/ms721572(v=VS.85).aspx">certificate revocation list</a> (CRL) distribution information extension and stores the resulting array in the COM object.


## -parameters




### -param strBinary [in]

An ASN.1-encoded CRL distribution information extension.


## -returns



<h3>VB</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.




## -remarks



This method places the decoded contents of <i>strBinary</i> into the object's array of CRL distribution information points. If the object's array already contains data, this existing content will be freed, and the array will be loaded with the decoded values.


#### Examples

For an example that uses the <b>Decode</b> method, see the <a href="https://msdn.microsoft.com/en-us/library/Aa383932(v=VS.85).aspx">ICertEncodeCRLDistInfo::Encode</a> method.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa383911(v=VS.85).aspx">ICertEncodeCRLDistInfo</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa383932(v=VS.85).aspx">ICertEncodeCRLDistInfo::Encode</a>
 

 

