---
UID: NN:certadm.IOCSPAdmin
title: IOCSPAdmin
author: windows-sdk-content
description: Provides functionality to manage an Online Certificate Status Protocol (OCSP) responder server.
old-location: security\iocspadmin.htm
tech.root: seccrypto
ms.assetid: cf76e934-07a2-46de-b2cf-7f6d3e274d71
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOCSPAdmin, IOCSPAdmin interface [Security], IOCSPAdmin interface [Security],described, OCSPAdmin object, certadm/IOCSPAdmin, security.iocspadmin
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: certadm.h
req.include-header: 
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
 - IOCSPAdmin
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCSPAdmin interface


## -description


The <b>IOCSPAdmin</b> interface provides functionality to manage an Online Certificate Status Protocol (OCSP) responder server. Implement this interface to manage individual responder server properties and <a href="https://msdn.microsoft.com/en-us/library/ms721572(v=VS.85).aspx">certification authority</a> (CA) definitions. After creating an instance of this interface, you call <a href="https://msdn.microsoft.com/en-us/library/Aa386317(v=VS.85).aspx">GetConfiguration</a> to connect to a responder service and initialize an <b>OCSPAdmin</b> object. Each <b>OCSPAdmin</b> object corresponds to one physical responder server.
<div class="alert"><b>Note</b>  This interface does not include functionality to  create or parse certificate status requests.</div><div> </div>In C++, you create an instance of this interface by calling the <b>CoCreateInstance</b> function with the <b>CLSID_OCSPAdmin</b> class identifier.

In Visual Basic Scripting Edition, you create an instance of the <b>OCSPAdmin</b> object.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IOCSPAdmin</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IOCSPAdmin</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Properties</a></li>
</ul>

## -members

The <b>IOCSPAdmin</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386317(v=VS.85).aspx">GetConfiguration</a>
</td>
<td align="left" width="63%">
Connects to a responder server and initializes an <b>OCSPAdmin</b> object with the configuration information from the server.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb394789(v=VS.85).aspx">GetHashAlgorithms</a>
</td>
<td align="left" width="63%">
Gets a list of hash-algorithm names. The responder server uses one of the named algorithms to sign OCSP responses for a given CA configuration.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386319(v=VS.85).aspx">GetMyRoles</a>
</td>
<td align="left" width="63%">
Gets the access mask of privilege roles for a user on a given responder server.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb394790(v=VS.85).aspx">GetSecurity</a>
</td>
<td align="left" width="63%">
Gets security descriptor information for a responder server.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb394791(v=VS.85).aspx">GetSigningCertificates</a>
</td>
<td align="left" width="63%">
Gets the signing certificates that are available on a responder server for a given CA certificate.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb394792(v=VS.85).aspx">Ping</a>
</td>
<td align="left" width="63%">
Tests a DCOM connection with a responder service.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386327(v=VS.85).aspx">SetConfiguration</a>
</td>
<td align="left" width="63%">
Updates a responder service  with configuration changes.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb394793(v=VS.85).aspx">SetSecurity</a>
</td>
<td align="left" width="63%">
Updates security descriptor information for an OCSP responder server.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IOCSPAdmin</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/Aa386323(v=VS.85).aspx">OCSPCAConfigurationCollection</a>


</td>
<td align="left" width="63%">
Gets an instance of an <a href="https://msdn.microsoft.com/en-us/library/Aa386323(v=VS.85).aspx">OCSPCAConfigurationCollection</a> object. This object represents the set of certificates for which a responder service can handle status requests.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/Aa386325(v=VS.85).aspx">OCSPServiceProperties</a>


</td>
<td align="left" width="63%">
Gets  an instance of a <a href="https://msdn.microsoft.com/en-us/library/Aa386394(v=VS.85).aspx">OCSPPropertyCollection</a> object. This object represents the attributes of a responder service.

</td>
</tr>
</table> 


## -remarks



The following table disambiguates the various properties used in the Microsoft OCSP architecture.

<table>
<tr>
<th>Architecture</th>
<th>Scope</th>
<th>Information types</th>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Aa386325(v=VS.85).aspx">OCSPServiceProperties</a>
</td>
<td>Governs general responder-service behavior for every CA.</td>
<td>
<ul>
<li>Proxy</li>
<li>Audit</li>
<li>Security configurations</li>
</ul>
</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Aa386323(v=VS.85).aspx">OCSPCAConfigurationCollection</a>
</td>
<td>Governs response behavior for a specific CA.</td>
<td>
<ul>
<li>CA</li>
<li>Hash algorithm</li>
<li>Certificate signing</li>
<li>Revocation provider configurations</li>
</ul>
</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Aa386372(v=VS.85).aspx">ProviderProperties</a>
</td>
<td>Governs behavior of a revocation information provider that is specific to a particular <a href="https://msdn.microsoft.com/en-us/library/Aa386328(v=VS.85).aspx">OCSPCAConfiguration</a>.</td>
<td>
<ul>
<li>Certificate revocation lists (CRLs)</li>
<li>Refresh interval</li>
</ul>
</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

