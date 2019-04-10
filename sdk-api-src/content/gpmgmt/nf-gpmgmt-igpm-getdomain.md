---
UID: NF:gpmgmt.IGPM.GetDomain
title: IGPM::GetDomain (gpmgmt.h)
author: windows-sdk-content
description: Creates and returns a GPMDomain object that corresponds to the specified domain.
old-location: gpmc\igpm_getdomain.htm
tech.root: gpmc
ms.assetid: 32aee72f-96fa-4ebd-9ff7-643972b82cf6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GPM object [GPMC],GetDomain method, GetDomain, GetDomain method [GPMC], GetDomain method [GPMC],GPM object, GetDomain method [GPMC],IGPM interface, IGPM interface [GPMC],GetDomain method, IGPM.GetDomain, IGPM::GetDomain, _win32_igpm_getdomain, gpmc.igpm_getdomain, gpmgmt/IGPM::GetDomain
ms.topic: method
req.header: gpmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Gpmgmt.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Gpmgmt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gpmgmt.dll
api_name:
 - IGPM.GetDomain
 - GPM.GetDomain
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IGPM::GetDomain

## -description


Creates and returns a 
<a href="https://msdn.microsoft.com/c3639f07-7c8c-4440-ade4-b58abd2586d6">GPMDomain</a> object that corresponds to the specified domain.

The object allows you to do the following:
<ul>
<li>Create, query, and restore Group Policy objects (GPOs)</li>
<li>Search scope of management (SOM) objects</li>
<li>Search and retrieve Windows Management Instrumentation (WMI) filters</li>
</ul>

## -parameters




### -param bstrDomain [in]

Name of the domain specified as a string. This must be a full Domain Name System (DNS) name, such as contoso.com.


### -param bstrDomainController [in]

If specified, the name of the domain controller to use with the domain. The name can be a DNS name or a NetBIOS name. Otherwise, the method uses the primary domain controller (PDC). For more information, see the <i>lDCFlags</i> parameter.

<b>Scripting:  </b>This parameter must pass an empty string ("") when a domain controller is not specified.


### -param lDCFlags [in]

Flags to use to locate the domain controller for the domain. You can specify <b>GPM_USE_ANYDC</b>, <b>GPM_USE_PDC</b>, or <b>GPM_DONOTUSE_W2KDC</b>.

If this parameter is set to zero, and a <i>bstrDomainController</i> is specified, the method uses the specified <i>bstrDomainController</i>. Otherwise, the method uses the PDC.


### -param pIGPMDomain [out]

Address of a pointer to the 
<a href="https://msdn.microsoft.com/c3639f07-7c8c-4440-ade4-b58abd2586d6">IGPMDomain</a> interface.


## -returns



<h3>C++</h3>
Returns <b>S_OK</b> if successful. Returns a failure code if an error occurs.

<h3>JScript</h3>
Returns a reference to a <b>GPMDomain</b> object.

<h3>VB</h3>
Returns a reference to a <b>GPMDomain</b> object.




## -remarks

>**Important:** When calling this function, underlying LDAP traffic is encrypted using Kerberos, not SSL.

This method does not allow you to search site SOMs. Call the 
<a href="https://msdn.microsoft.com/0a1b8975-cd73-49e6-83b9-f6af296276cb">IGPM::GetSitesContainer</a> method to perform this type of query.




## -see-also




<a href="https://msdn.microsoft.com/2780760e-7114-46b0-a264-00ed58a556cb">IGPM</a>



<a href="https://msdn.microsoft.com/c3639f07-7c8c-4440-ade4-b58abd2586d6">IGPMDomain</a>
 

 

