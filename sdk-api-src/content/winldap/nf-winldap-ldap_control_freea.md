---
UID: NF:winldap.ldap_control_freeA
title: ldap_control_freeA function (winldap.h)
author: windows-sdk-content
description: The ldap_control_free function frees an LDAPControl structure.
old-location: ldap\ldap_control_free.htm
tech.root: ldap
ms.assetid: 10729355-8f80-477b-acc8-705db72cebdb
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "_ldap_ldap_control_free, ldap.ldap__control__free, ldap.ldap_control_free, ldap_control_free, ldap_control_free function [LDAP], ldap_control_freeA, ldap_control_freeW, winldap/ldap_control_free, winldap/ldap_control_freeA, winldap/ldap_control_freeW"
ms.topic: function
req.header: winldap.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: ldap_control_freeW (Unicode) and ldap_control_freeA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wldap32.lib
req.dll: Wldap32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Wldap32.dll
api_name:
 - ldap_control_free
 - ldap_control_freeA
 - ldap_control_freeW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ldap_control_freeA function


## -description


The <b>ldap_control_free</b> function frees an 
   <a href="https://msdn.microsoft.com/c0b4d712-021d-46f3-8bda-aaf660ec1acc">LDAPControl</a> structure.


## -parameters




### -param Controls

TBD




#### - Control [in]

The <a href="https://msdn.microsoft.com/c0b4d712-021d-46f3-8bda-aaf660ec1acc">LDAPControl</a> structure to free.


## -returns



If the function succeeds, <b>LDAP_SUCCESS</b> is returned.

If the function fails, an error code is returned. For more information, see 
       <a href="https://msdn.microsoft.com/822411b7-fc49-4b93-8e54-353350ed5de9">Return Values</a>.




## -remarks



Use this function to free an <a href="https://msdn.microsoft.com/c0b4d712-021d-46f3-8bda-aaf660ec1acc">LDAPControl</a> structure 
     previously allocated by an LDAP function call, such as one allocated by a call to 
     <a href="https://msdn.microsoft.com/b3b1f3bd-7eb3-4f76-921c-386562dae2e2">ldap_create_page_control</a> or 
     <a href="https://msdn.microsoft.com/f4305aa9-e967-45a8-8b8b-49b1e60994e8">ldap_create_vlv_control</a>.

<div class="alert"><b>Note</b>  This function should only be used to free a control created internally by LDAP API functions. It is not used 
     to free memory that is explicitly allocated by the user program.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/7a0040ea-f8f3-4378-8371-49768714d762">Functions</a>



<a href="https://msdn.microsoft.com/c0b4d712-021d-46f3-8bda-aaf660ec1acc">LDAPControl</a>



<a href="https://msdn.microsoft.com/822411b7-fc49-4b93-8e54-353350ed5de9">Return Values</a>



<a href="https://msdn.microsoft.com/b3b1f3bd-7eb3-4f76-921c-386562dae2e2">ldap_create_page_control</a>



<a href="https://msdn.microsoft.com/f4305aa9-e967-45a8-8b8b-49b1e60994e8">ldap_create_vlv_control</a>
 

 

