---
UID: NF:winldap.ldap_modrdn2_sA
title: ldap_modrdn2_sA function (winldap.h)
author: windows-sdk-content
description: The ldap_modrdn2_s function changes the relative distinguished name of an LDAP entry.
old-location: ldap\ldap_modrdn2_s.htm
tech.root: ldap
ms.assetid: a2cf121d-4e84-4195-9080-3b6c0c4cea82
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "_ldap_ldap_modrdn2_s, ldap.ldap__modrdn2__s, ldap.ldap_modrdn2_s, ldap_modrdn2_s, ldap_modrdn2_s function [LDAP], ldap_modrdn2_sA, ldap_modrdn2_sW, winldap/ldap_modrdn2_s, winldap/ldap_modrdn2_sA, winldap/ldap_modrdn2_sW"
ms.topic: function
req.header: winldap.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: ldap_modrdn2_sW (Unicode) and ldap_modrdn2_sA (ANSI)
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
 - ldap_modrdn2_s
 - ldap_modrdn2_sA
 - ldap_modrdn2_sW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ldap_modrdn2_sA function


## -description


The <b>ldap_modrdn2_s</b> function changes the relative distinguished name of an LDAP entry.

This function is obsolete. For LDAP 3 or later, use the 
<a href="https://msdn.microsoft.com/73633a71-ebe6-4169-a9ff-17151d90ebcd">ldap_rename_ext</a> or 
<a href="https://msdn.microsoft.com/85a605f9-d075-4b1d-bfcb-a75c9e7f3023">ldap_rename_ext_s</a> functions.


## -parameters




### -param ExternalHandle [in]

The session handle.


### -param DistinguishedName [in]

A pointer to a null-terminated string that contains the distinguished name to change.


### -param NewDistinguishedName [in]

A pointer to a null-terminated string that contains the new relative distinguished name to give the entry.


### -param DeleteOldRdn [in]

<b>TRUE</b> if the old relative distinguished name should be deleted; <b>FALSE</b> if the old relative distinguished name should be retained.


## -returns



If the function succeeds, the return value is <b>LDAP_SUCCESS</b>.

If the function fails, it returns an error code. For more information, see 
<a href="https://msdn.microsoft.com/822411b7-fc49-4b93-8e54-353350ed5de9">Return Values</a>.




## -remarks



Be aware that the various <a href="https://msdn.microsoft.com/7a85eb4d-dcb1-4a5b-a7df-1d726215bde3">ldap_modrdn</a> functions allow you to change only the relative distinguished name, which is the least significant component of the object's distinguished name. Effective with version 3, LDAP provides the Modify Distinguished Name protocol operation that allows access to name-change functions. This feature is available by calling 
<a href="https://msdn.microsoft.com/73633a71-ebe6-4169-a9ff-17151d90ebcd">ldap_rename_ext</a> or 
<a href="https://msdn.microsoft.com/85a605f9-d075-4b1d-bfcb-a75c9e7f3023">ldap_rename_ext_s</a>. These functions are recommended, rather than the <b>ldap_modrdn2_s</b> function, to change an entry name.

<div class="alert"><b>Note</b>  When connecting to an LDAP 2 server, the application must perform a bind operation, by calling one of the 
<a href="https://msdn.microsoft.com/889636f2-3dd0-4027-aa35-d7b7930d9e69">ldap_bind</a> or 
<a href="https://msdn.microsoft.com/13fc47c5-094b-4a91-8e5f-bfff8c72b431">ldap_simple_bind</a> routines, before attempting any other operations.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/7a0040ea-f8f3-4378-8371-49768714d762">Functions</a>



<a href="https://msdn.microsoft.com/ad7be3a1-663c-489e-8eb3-1aea910ee366">Modifying a Directory Entry</a>



<a href="https://msdn.microsoft.com/889636f2-3dd0-4027-aa35-d7b7930d9e69">ldap_bind</a>



<a href="https://msdn.microsoft.com/7bf7370f-a5e6-474e-8fe9-e6895ef48ab5">ldap_modrdn2</a>



<a href="https://msdn.microsoft.com/73633a71-ebe6-4169-a9ff-17151d90ebcd">ldap_rename_ext</a>



<a href="https://msdn.microsoft.com/85a605f9-d075-4b1d-bfcb-a75c9e7f3023">ldap_rename_ext_s</a>



<a href="https://msdn.microsoft.com/13fc47c5-094b-4a91-8e5f-bfff8c72b431">ldap_simple_bind</a>
 

 

