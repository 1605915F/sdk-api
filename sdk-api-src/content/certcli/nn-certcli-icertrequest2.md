---
UID: NN:certcli.ICertRequest2
title: ICertRequest2
author: windows-sdk-content
description: Provide communications between a client or intermediary application and Certificate Services.
old-location: security\icertrequest2.htm
tech.root: seccrypto
ms.assetid: 8587a682-27a5-4f26-b4bb-7088e4e5d8d3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICertRequest2, ICertRequest2 interface [Security], ICertRequest2 interface [Security],described, _certsrv_icertrequest2, certcli/ICertRequest2, security.icertrequest2
ms.topic: interface
req.header: certcli.h
req.include-header: Certsrv.h
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
req.lib: Certidl.lib
req.dll: Certcli.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certcli.dll
api_name:
 - ICertRequest2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertRequest2 interface


## -description


The <b>ICertRequest2</b> interface is one of two interfaces that  provide communications between a client or intermediary application and <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">Certificate Services</a>.

Client and intermediary applications can call the  <a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest2</a> methods to perform the following tasks:<ul>
<li>Submit certificate request.</li>
<li>Retrieve the disposition, last status, and identifier of a request.</li>
<li>Retrieve the certificate issued for the request.</li>
<li>Retrieve pending certificates for previous requests.</li>
<li>Retrieve the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certification authority</a> (CA) certificate for the Certificate Services server.</li>
<li>Retrieve the CA property value, display name, and any flags associated with the property.</li>
<li>Retrieve the cached response data returned by the server.</li>
<li>Retrieve error message text for an <b>HRESULT</b> error code.</li>
</ul>


<b>ICertRequest2</b> is defined in Certcli.h. When you create your program, however, use Certsrv.h as the include file. Certcli.dll provides the <b>ICertRequest2</b> interface. The type information for this interface is also in Certclil.dll, which is shipped with the Platform Software Development Kit (SDK).

Certificate Services interfaces support both apartment-threading and free-threading models. For better throughput, free threading is recommended.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICertRequest2</b> interface inherits from <a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a> and <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>. <b>ICertRequest2</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ICertRequest2</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/711fdcec-0a07-4559-a577-1eb73053dd38">GetCACertificate</a>
</td>
<td align="left" width="63%">
Returns the CA certificate for the Certificate Services server.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/093d657d-2d9c-4973-a71b-5b134cc35034">GetCAProperty</a>
</td>
<td align="left" width="63%">
Retrieves a property value from the CA. This method's functionality is identical to 
<a href="https://msdn.microsoft.com/8eaa2e36-4358-4abd-a7c2-2c9768766597">ICertAdmin2::GetCAProperty</a>.</p> (Inherited from <b>ICertRequest2</b><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5c294758-b2aa-497b-8377-6c5987576f82">GetCAPropertyDisplayName</a>
</td>
<td align="left" width="63%">
Retrieves the display name for a property. This method's functionality is identical to 
<a href="https://msdn.microsoft.com/8f879b94-d15a-48e6-9e71-a24c1c39c618">ICertAdmin2::GetCAPropertyDisplayName</a>.</p> (Inherited from <b>ICertRequest2</b><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bdc6ab73-a0b4-44cd-9e46-c453dcb45a41">GetCAPropertyFlags</a>
</td>
<td align="left" width="63%">
Retrieves the property flags (denoting data type and indexed status) for a property. This method's functionality is identical to 
<a href="https://msdn.microsoft.com/6f38bea1-e278-4085-b321-05f6765cc676">ICertAdmin2::GetCAPropertyFlags</a>.</p> (Inherited from <b>ICertRequest2</b><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ba8fc725-c376-4e66-8417-777ce13f2954">GetCertificate</a>
</td>
<td align="left" width="63%">
Returns the certificate issued for the request.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c3639cf6-c70f-4f15-a0ed-e60abe2955cb">GetDispositionMessage</a>
</td>
<td align="left" width="63%">
Gets a human-readable message giving the current disposition of the certificate request.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/eeecaeec-2e06-4d4b-9b85-5fb3ef90944a">GetErrorMessageText</a>
</td>
<td align="left" width="63%">
Retrieves message text for a given <b>HRESULT</b> error code.</p> (Inherited from <b>ICertRequest2</b><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1ee979b7-2d2a-4140-8eef-5e3a5e0c132c">GetFullResponseProperty</a>
</td>
<td align="left" width="63%">
Retrieves the cached response data returned by the server.</p> (Inherited from <b>ICertRequest2</b><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ea7f6013-a55d-4a76-9c9e-df180ba9bb79">GetIssuedCertificate</a>
</td>
<td align="left" width="63%">
Retrieves the disposition of a certificate request.</p> (Inherited from <b>ICertRequest2</b><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ebe5cfa7-6bfd-4454-9272-64e3b1bf0ae2">GetLastStatus</a>
</td>
<td align="left" width="63%">
Gets the last return code for this request.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bb808834-7083-4b14-bce7-96b6fef242cc">GetRequestId</a>
</td>
<td align="left" width="63%">
Gets the current internal request number for the request and subsequent certificate.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/07a9ac57-f90e-4c5c-b563-8aebbcf8f42e">RetrievePending</a>
</td>
<td align="left" width="63%">
Attempts to retrieve the certificate issued for an earlier request, that may have initially been made pending.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/22ae8d39-3f16-4f7d-94a0-aa68b03aaa0b">Submit</a>
</td>
<td align="left" width="63%">
Submits a request to the Certificate Services server.</p> (Inherited from <b>ICertRequest2</b><a href="https://msdn.microsoft.com/2f371aa6-492e-41ba-8455-66e9d5f5da44">ICertRequest</a><b>CCertRequest</b>)</td>
</tr>
</table> 

