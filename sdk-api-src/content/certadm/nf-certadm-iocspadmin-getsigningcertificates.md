---
UID: NF:certadm.IOCSPAdmin.GetSigningCertificates
title: IOCSPAdmin::GetSigningCertificates (certadm.h)
author: windows-sdk-content
description: Gets the signing certificates that are available on a responder server for a given certification authority (CA) certificate.
old-location: security\iocspadmin_getsigningcertificates.htm
tech.root: SecCrypto
ms.assetid: 762dc32f-90d4-4e88-a3cc-e77e729f0a98
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetSigningCertificates, GetSigningCertificates method [Security], GetSigningCertificates method [Security],IOCSPAdmin interface, IOCSPAdmin interface [Security],GetSigningCertificates method, IOCSPAdmin.GetSigningCertificates, IOCSPAdmin::GetSigningCertificates, certadm/IOCSPAdmin::GetSigningCertificates, security.iocspadmin_getsigningcertificates
ms.topic: method
req.header: certadm.h
req.include-header: Certsrv.h
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certadm.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Certadm.lib
req.dll: Certadm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certadm.dll
api_name:
 - IOCSPAdmin.GetSigningCertificates
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCSPAdmin::GetSigningCertificates


## -description


The <b>GetSigningCertificates</b> method  gets the signing certificates that are available on a responder server for a given <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certification authority</a> (CA) certificate. This method only returns signing certificates from the <b>CERT_SYSTEM_STORE_LOCAL_MACHINE</b> system store for the specified server.


## -parameters




### -param bstrServerName [in]

A string that contains the responder-server name.


### -param pCACertVar [in]

The CA certificate for which to retrieve signing certificates.


### -param pVal [out]


## -returns



<h3>C++</h3>
 If the method succeeds, it returns <b>S_OK</b>.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.

<h3>VB</h3>
The available signing certificates.



## -remarks



Each signing certificate has the following properties:

<ul>
<li>Signed by the CA specified by the <i>pCACertVar</i> parameter</li>
<li>Includes the Online Certificate Status Protocol (OCSP) signing (<b>XCN_OID_PKIX_KP_OCSP_SIGNING</b>) extension</li>
<li>Has not expired</li>
<li>Responder server can access the certificate private key</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/cf76e934-07a2-46de-b2cf-7f6d3e274d71">IOCSPAdmin</a>
 

 

