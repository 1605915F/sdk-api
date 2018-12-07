---
UID: NN:casetup.IMSCEPSetup
title: IMSCEPSetup
author: windows-sdk-content
description: Defines functionality to install and uninstall a Network Device Enrollment Service (NDES) role on a Certificate Services computer.
old-location: security\imscepsetup.htm
tech.root: seccrypto
ms.assetid: 328c6c04-7ade-4b64-bd8a-4314b6e8dc78
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSCEPSetup, IMSCEPSetup interface [Security], IMSCEPSetup interface [Security],described, casetup/IMSCEPSetup, security.imscepsetup
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: casetup.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Casetup.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Certocm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certocm.dll
api_name:
 - IMSCEPSetup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSCEPSetup interface


## -description


The <b>IMSCEPSetup</b> interface defines functionality to install and uninstall a Network Device Enrollment Service (NDES) role on a Certificate Services computer. Implement this interface to provide a custom setup program for installing and uninstalling this role.

Microsoft provides an implementation of this interface in the <b>CMSCEPSetup</b> class. For installation, you must call <a href="https://msdn.microsoft.com/en-us/library/Bb736408(v=VS.85).aspx">InitializeDefaults</a> before accessing any properties or calling any other methods on the <b>CMSCEPSetup</b> object.

In C++, you create an instance of this interface by calling the <b>CoCreateInstance</b> function with the <b>CLSID_CMSCEPSetup</b> class identifier.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMSCEPSetup</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IMSCEPSetup</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Properties</a></li>
</ul>

## -members

The <b>IMSCEPSetup</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb736405(v=VS.85).aspx">GetKeyLengthList</a>
</td>
<td align="left" width="63%">
Gets the list of <a href="https://msdn.microsoft.com/en-us/library/ms721590(v=VS.85).aspx">key lengths</a> supported by the specified CSP.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb736406(v=VS.85).aspx">GetMSCEPSetupProperty</a>
</td>
<td align="left" width="63%">
Gets a property value for an NDES configuration.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb736407(v=VS.85).aspx">GetProviderNameList</a>
</td>
<td align="left" width="63%">
Gets the list of <a href="https://msdn.microsoft.com/en-us/library/ms721572(v=VS.85).aspx">cryptographic service providers</a> (CSPs) that provide asymmetric key signature and exchange algorithms on the computer.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb736408(v=VS.85).aspx">InitializeDefaults</a>
</td>
<td align="left" width="63%">
Initializes a <b>CMSCEPSetup</b> object with default values to enable installation of an NDES role.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/26ed36bd-8d27-42ce-81a5-a980fdebf5af">Install</a>
</td>
<td align="left" width="63%">
Installs an NDES role as configured in the <b>CMSCEPSetup</b> object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/90ce2ea5-e531-4787-954a-cd4d09ba753e">IsMSCEPStoreEmpty</a>
</td>
<td align="left" width="63%">
This method always returns <b>VARIANT_TRUE</b>. It should not be used.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/8989ebde-0d33-4f9a-a4dc-82562eab5976">PostUnInstall</a>
</td>
<td align="left" width="63%">
This method is not implemented. It is reserved for future use.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7c9ff619-7c26-4dfb-aeac-fa80a1050cf0">PreUnInstall</a>
</td>
<td align="left" width="63%">
Removes registry and IIS settings for the NDES role.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/32d09bdc-e8e8-4368-9f51-cc7ba170c8a0">SetAccountInformation</a>
</td>
<td align="left" width="63%">
Sets the user account information used by the IIS NDES extension to perform enrollment on behalf of network devices.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/868f3e5f-1345-414b-a75f-d2e68213469b">SetMSCEPSetupProperty</a>
</td>
<td align="left" width="63%">
Sets a property value for an NDES configuration.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMSCEPSetup</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/3edec047-1034-44c8-bac5-f3593cb1b66b">MSCEPErrorId</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Gets the ID for additional error information related to a failed NDES specification. Any method call on the parent object resets this property.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/Bb736412(v=VS.85).aspx">MSCEPErrorString</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Gets the string data for additional error information related to a failed NDES specification. Any method call on the parent object resets this property.

</td>
</tr>
</table> 

