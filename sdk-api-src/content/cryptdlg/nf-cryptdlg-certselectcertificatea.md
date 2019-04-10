---
UID: NF:cryptdlg.CertSelectCertificateA
title: CertSelectCertificateA function (cryptdlg.h)
author: windows-sdk-content
description: Presents a dialog box that allows the user to select certificates from a set of certificates that match the given criteria.
old-location: security\certselectcertificate.htm
tech.root: SecCrypto
ms.assetid: 8160ea08-c7c0-40f5-8771-6603f768744b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CertSelectCertificate, CertSelectCertificate function [Security], CertSelectCertificateA, CertSelectCertificateW, cryptdlg/CertSelectCertificate, cryptdlg/CertSelectCertificateA, cryptdlg/CertSelectCertificateW, security.certselectcertificate
ms.topic: function
req.header: cryptdlg.h
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
req.dll: CryptDlg.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - CryptDlg.dll
api_name:
 - CertSelectCertificate
 - CertSelectCertificateA
 - CertSelectCertificateW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CertSelectCertificateA function


## -description


The <b>CertSelectCertificate</b> function  presents a dialog box that allows the user to select certificates from a set of certificates that match the given criteria.
<div class="alert"><b>Note</b>  This function has no associated import library. You must use the <a href="https://msdn.microsoft.com/d936b4dd-058c-48e1-834b-b47ef6d8ef65">LoadLibrary</a> and <a href="https://msdn.microsoft.com/a0d7fc09-f888-4f46-a571-d3719a627597">GetProcAddress</a> functions to dynamically link to CryptDlg.dll.</div><div> </div>

## -parameters




### -param pCertSelectInfo [in, out]

A pointer to a <a href="https://msdn.microsoft.com/49184872-d636-4e55-8e32-0f38b49b5c21">CERT_SELECT_STRUCT</a> structure that contains criteria that control the displayed certificates for selection and receives the selected certificate.


## -returns



If the function succeeds, the return value is <b>TRUE</b>.

If the function fails, the return value is <b>FALSE</b>. For extended error information, call the 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function.




## -see-also




<a href="https://msdn.microsoft.com/49184872-d636-4e55-8e32-0f38b49b5c21">CERT_SELECT_STRUCT</a>
 

 

