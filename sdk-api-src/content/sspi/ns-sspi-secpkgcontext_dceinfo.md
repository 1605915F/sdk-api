---
UID: NS:sspi._SecPkgContext_DceInfo
title: SecPkgContext_DceInfo
author: windows-sdk-content
description: The SecPkgContext_DceInfo structure contains authorization data used by DCE services. The QueryContextAttributes (General) function uses this structure.
old-location: security\secpkgcontext_dceinfo.htm
tech.root: secauthn
ms.assetid: 490688d0-efdd-4a40-88b9-eb53ff592d2a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSecPkgContext_DceInfo, PSecPkgContext_DceInfo, PSecPkgContext_DceInfo structure pointer [Security], SecPkgContext_DceInfo, SecPkgContext_DceInfo structure [Security], _ssp_secpkgcontext_dceinfo, security.secpkgcontext_dceinfo, sspi/PSecPkgContext_DceInfo, sspi/SecPkgContext_DceInfo"
ms.topic: struct
req.header: sspi.h
req.include-header: Security.h
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
 - Sspi.h
api_name:
 - SecPkgContext_DceInfo
product: Windows
targetos: Windows
req.typenames: SecPkgContext_DceInfo, *PSecPkgContext_DceInfo
req.redist: 
---

# SecPkgContext_DceInfo structure


## -description


The <b>SecPkgContext_DceInfo</b> structure contains authorization data used by DCE services. The 
<a href="https://msdn.microsoft.com/67bc087f-7519-4c8a-9b34-b3ecd306a334">QueryContextAttributes (General)</a> function uses this structure.


## -struct-fields




### -field AuthzSvc

Specifies the authorization service used. For DCE use only.


### -field pPac

Pointer to package-specific authorization data.


## -see-also




<a href="https://msdn.microsoft.com/67bc087f-7519-4c8a-9b34-b3ecd306a334">QueryContextAttributes (General)</a>
 

 

