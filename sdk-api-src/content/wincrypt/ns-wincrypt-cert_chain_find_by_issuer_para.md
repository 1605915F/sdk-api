---
UID: NS:wincrypt._CERT_CHAIN_FIND_BY_ISSUER_PARA
title: CERT_CHAIN_FIND_BY_ISSUER_PARA
author: windows-sdk-content
description: Contains information used in the CertFindChainInStore function to build certificate chains.
old-location: security\cert_chain_find_by_issuer_para.htm
tech.root: seccrypto
ms.assetid: 7dee640e-6bad-4d3c-910f-da928a8682c9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCERT_CHAIN_FIND_BY_ISSUER_PARA, *PCERT_CHAIN_FIND_ISSUER_PARA, AT_KEYEXCHANGE, AT_SIGNATURE, CERT_CHAIN_FIND_BY_ISSUER_PARA, CERT_CHAIN_FIND_BY_ISSUER_PARA structure [Security], CERT_CHAIN_FIND_ISSUER_PARA, _CERT_CHAIN_FIND_BY_ISSUER_PARA, _CERT_CHAIN_FIND_BY_ISSUER_PARA structure [Security], _crypto2_cert_chain_find_by_issuer_para, security.cert_chain_find_by_issuer_para, wincrypt/CERT_CHAIN_FIND_BY_ISSUER_PARA"
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Wincrypt.h
api_name:
 - _CERT_CHAIN_FIND_BY_ISSUER_PARA
product: Windows
targetos: Windows
req.typenames: CERT_CHAIN_FIND_ISSUER_PARA, *PCERT_CHAIN_FIND_ISSUER_PARA, CERT_CHAIN_FIND_BY_ISSUER_PARA, *PCERT_CHAIN_FIND_BY_ISSUER_PARA
req.redist: 
---

# CERT_CHAIN_FIND_BY_ISSUER_PARA structure


## -description


The <b>CERT_CHAIN_FIND_BY_ISSUER_PARA</b> structure contains information used in the <a href="https://msdn.microsoft.com/698cece8-71a8-4bfa-8ee6-8035a6dcbe05">CertFindChainInStore</a> function to build certificate chains.


## -struct-fields




### -field cbSize

Contains the size of this structure, in bytes. This size should not be hard-coded. It should be set at compile time by using the <b>sizeof</b> operator as shown in the following example.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>CERT_CHAIN_FIND_BY_ISSUER_PARA findParams;
findParams.cbSize = sizeof(CERT_CHAIN_FIND_BY_ISSUER_PARA);</pre>
</td>
</tr>
</table></span></div>

### -field pszUsageIdentifier

A pointer to a null-terminated ANSI string that contains the usage identifier to be matched. If this member is <b>NULL</b>, a certificate with any usage can be a match.


### -field dwKeySpec

Contains the key specification value to be matched. This can be one of the following values. If this parameter is zero, any certificate can match.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="AT_KEYEXCHANGE"></a><a id="at_keyexchange"></a><dl>
<dt><b>AT_KEYEXCHANGE</b></dt>
<dt>0x01</dt>
</dl>
</td>
<td width="60%">
The key can be used to encrypt or sign depending on the algorithm.

</td>
</tr>
<tr>
<td width="40%"><a id="AT_SIGNATURE"></a><a id="at_signature"></a><dl>
<dt><b>AT_SIGNATURE</b></dt>
<dt>0x02</dt>
</dl>
</td>
<td width="60%">
The key can be used for signing.

</td>
</tr>
</table>
 


### -field dwAcquirePrivateKeyFlags

When the <i>dwFindFlags</i> parameter of the <a href="https://msdn.microsoft.com/698cece8-71a8-4bfa-8ee6-8035a6dcbe05">CertFindChainInStore</a> function contains <b>CERT_CHAIN_FIND_BY_ISSUER_COMPARE_KEY_FLAG</b>, the <a href="https://msdn.microsoft.com/53c9aec9-701d-4c21-9814-d344a8dde0c1">CryptAcquireCertificatePrivateKey</a> function is called to do the public key comparison. In this case, this member is passed as the <i>dwFlags</i> parameter of the <b>CryptAcquireCertificatePrivateKey</b> function. For possible values for this member and their meanings, see the <i>dwFlags</i> parameter of the <b>CryptAcquireCertificatePrivateKey</b> function.


### -field cIssuer

Contains the number of elements in the <b>rgIssuer</b> array. If this member is zero, any issuer can be a match.


### -field rgIssuer

An array of <a href="https://msdn.microsoft.com/28dba6ef-939f-4789-9789-ee6e0fef0177">X.509</a>, <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">Abstract Syntax Notation One</a> (ASN.1) encoded issuer name <a href="https://msdn.microsoft.com/2e570727-7da0-4e17-bf5d-6fe0e6aef65b">BLOBs</a> to match. If this member is <b>NULL</b> or the callback function returns <b>TRUE</b>, a new element is added to the chain for the certificate having a <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">private key</a> with the specified KeySpec and <a href="https://msdn.microsoft.com/f1caccd2-3453-448e-b194-bf899eff8091">enhanced key usage</a>.


### -field pfnFindCallback

A pointer to a <a href="https://msdn.microsoft.com/004c4caa-0063-41a3-8d6d-8b3a769b4112">CertChainFindByIssuerCallback</a> callback function that allows the application to filter the certificates that chains are created for. If this member is <b>NULL</b>, a chain is built for every certificate found. If this member is not <b>NULL</b>, a chain will be built for the certificate found based on the return value of the callback function.


### -field pvFindArg

An application-defined value that will be passed as the <i>pvFindArg</i> parameter of the <a href="https://msdn.microsoft.com/004c4caa-0063-41a3-8d6d-8b3a769b4112">CertChainFindByIssuerCallback</a> callback function pointed to by the <b>pfnFindCallback</b> member of this structure.


### -field pdwIssuerChainIndex

A pointer to a <b>DWORD</b> value that receives the zero-based index of the chain that matches the issuer. If this member is <b>NULL</b>, it is not used.

If <b>cIssuer</b> is zero, this member is not used.

This member is only defined if the <b>CERT_CHAIN_FIND_BY_ISSUER_PARA_HAS_EXTRA_FIELDS</b> macro is defined.


### -field pdwIssuerElementIndex

A pointer to a <b>DWORD</b> value that receives the zero-based index of the element in the chain of the certificate of the issuer. If this member is <b>NULL</b>, it is not used.

If <b>cIssuer</b> is zero, this member is not used.

This  member is set to the index of the found certificate plus one to provide the index of  the certificate of the issuer. Because of this, a partial chain or a self-signed certificate that matches the name BLOB may cause <b>pdwIssuerElementIndex</b> to point past the last certificate in the chain. This situation can be detected by comparing the contents of <b>pdwIssuerElementIndex</b> with the <b>cElement</b> member of the <a href="https://msdn.microsoft.com/c130cab4-bf8d-429a-beb7-04cb5d37d466">CERT_SIMPLE_CHAIN</a> structure to make sure the index is valid.

This member is only defined if the <b>CERT_CHAIN_FIND_BY_ISSUER_PARA_HAS_EXTRA_FIELDS</b> macro is defined.


## -remarks



The <b>pdwIssuerChainIndex</b> and <b>pdwIssuerElementIndex</b> members are only available if the <b>CERT_CHAIN_FIND_BY_ISSUER_PARA_HAS_EXTRA_FIELDS</b> macro is defined. If the <b>CERT_CHAIN_FIND_BY_ISSUER_PARA_HAS_EXTRA_FIELDS</b> macro is defined, the application must initialize all unused fields to zero.


#### Examples

The following pseudocode shows how to use the <b>pdwIssuerChainIndex</b> and <b>pdwIssuerElementIndex</b> members of this structure to access the certificate of the issuer.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>CERT_CHAIN_FIND_BY_ISSUER_PARA findParams;
PCCERT_CHAIN_CONTEXT pChainContext = NULL;
DWORD dwChainIndex = 0;
DWORD dwElementIndex = 0;
findParams.pdwIssuerChainIndex = &amp;dwChainIndex;
findParams.pdwIssuerElementIndex = &amp;dwElementIndex;

pChainContext = CertFindChainInStore(
    hCertStore,
    X509_ASN_ENCODING,
    0,
    CERT_CHAIN_FIND_BY_ISSUER,
    (LPVOID)&amp;findParams,
    NULL);
if(pChainContext)
{
    // Make sure the element index is valid.
    if(dwElementIndex &lt; pChainContext-&gt;
        rgpChain[dwChainIndex]-&gt;cElement)
    {
        PCERT_CHAIN_ELEMENT pIssuerElement;
        pIssuerElement = pChainContext-&gt;
            rgpChain[dwChainIndex]-&gt;rgpElement[dwElementIndex];
       // ...
    }

    // Free the certificate chain.
    CertFreeCertificateChain(pChainContext);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/004c4caa-0063-41a3-8d6d-8b3a769b4112">CertChainFindByIssuerCallback</a>



<a href="https://msdn.microsoft.com/698cece8-71a8-4bfa-8ee6-8035a6dcbe05">CertFindChainInStore</a>



<a href="https://msdn.microsoft.com/53c9aec9-701d-4c21-9814-d344a8dde0c1">CryptAcquireCertificatePrivateKey</a>
 

 

