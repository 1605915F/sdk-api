---
UID: NS:sspi._SecPkgContext_PackageInfoA
title: "_SecPkgContext_PackageInfoA"
author: windows-sdk-content
description: The SecPkgContext_PackageInfo structure contains the name of a security support provider (SSP).
old-location: security\secpkgcontext_packageinfo.htm
tech.root: secauthn
ms.assetid: 94c21f22-d974-4ae5-beef-d4567e6ea7e1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSecPkgContext_PackageInfoA, PSecPkgContext_PackageInfo, PSecPkgContext_PackageInfo structure pointer [Security], SecPkgContext_PackageInfo, SecPkgContext_PackageInfo structure [Security], SecPkgContext_PackageInfoA, _SecPkgContext_PackageInfoA, _SecPkgContext_PackageInfoW, _ssp_secpkgcontext_packageinfo, security.secpkgcontext_packageinfo, sspi/PSecPkgContext_PackageInfo, sspi/SecPkgContext_PackageInfo"
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - SecPkgContext_PackageInfo
product: Windows
targetos: Windows
req.typenames: SecPkgContext_PackageInfoA, *PSecPkgContext_PackageInfoA
req.redist: 
---

# _SecPkgContext_PackageInfoA structure


## -description


The <b>SecPkgContext_PackageInfo</b> structure contains the name of a <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security support provider</a> (SSP). This structure is returned by the 
<a href="https://msdn.microsoft.com/67bc087f-7519-4c8a-9b34-b3ecd306a334">QueryContextAttributes (General)</a> function. It would most often be used when the SSP in use was established using the <a href="https://msdn.microsoft.com/28d229ef-53ce-4d17-aba0-3bbf51e3ff0c">Negotiate</a> <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security package</a>.


## -struct-fields




### -field PackageInfo

Pointer to a 
<a href="https://msdn.microsoft.com/d0bff3d8-63f1-4a4e-851f-177040af6bd2">SecPkgInfo</a> structure containing the name of the SSP in use.


## -see-also




<a href="https://msdn.microsoft.com/67bc087f-7519-4c8a-9b34-b3ecd306a334">QueryContextAttributes (General)</a>



<a href="https://msdn.microsoft.com/d0bff3d8-63f1-4a4e-851f-177040af6bd2">SecPkgInfo</a>
 

 

