---
UID: NF:certadm.IOCSPAdmin.SetSecurity
title: IOCSPAdmin::SetSecurity
author: windows-sdk-content
description: Updates security descriptor information for an Online Certificate Status Protocol (OCSP) responder server.
old-location: security\iocspadmin_setsecurity.htm
tech.root: SecCrypto
ms.assetid: 7ff94496-4347-4c08-8c71-0c53af902d9d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOCSPAdmin interface [Security],SetSecurity method, IOCSPAdmin.SetSecurity, IOCSPAdmin::SetSecurity, SetSecurity, SetSecurity method [Security], SetSecurity method [Security],IOCSPAdmin interface, certadm/IOCSPAdmin::SetSecurity, security.iocspadmin_setsecurity
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
 - IOCSPAdmin.SetSecurity
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCSPAdmin::SetSecurity


## -description


The <b>SetSecurity</b> method updates security descriptor information for an Online Certificate Status Protocol (OCSP) responder server.


## -parameters




### -param bstrServerName [in]

A string that contains the responder-server name.


### -param bstrVal [in]

A string that contains the security descriptor information to assign to the responder server.


## -remarks



This method calls the <a href="https://msdn.microsoft.com/c5654148-fb4c-436d-9378-a1168fc82607">ConvertStringSecurityDescriptorToSecurityDescriptor</a> function to create a security descriptor from a string in <a href="https://msdn.microsoft.com/0a226629-084c-40c5-bdd4-ad7355c807cf">Security Descriptor String Format</a>.




## -see-also




<a href="https://msdn.microsoft.com/cf76e934-07a2-46de-b2cf-7f6d3e274d71">IOCSPAdmin</a>
 

 

