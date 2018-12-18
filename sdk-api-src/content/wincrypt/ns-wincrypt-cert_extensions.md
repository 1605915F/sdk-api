---
UID: NS:wincrypt._CERT_EXTENSIONS
title: CERT_EXTENSIONS
author: windows-sdk-content
description: The CERT_EXTENSIONS structure contains an array of extensions.
old-location: security\cert_extensions.htm
tech.root: seccrypto
ms.assetid: b393ef08-cedb-4840-a427-10ead315d6ea
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCERT_EXTENSIONS, CERT_EXTENSIONS, CERT_EXTENSIONS structure [Security], PCERT_EXTENSIONS, PCERT_EXTENSIONS structure pointer [Security], _crypto2_cert_extensions, security.cert_extensions, wincrypt/CERT_EXTENSIONS, wincrypt/PCERT_EXTENSIONS"
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
 - CERT_EXTENSIONS
product: Windows
targetos: Windows
req.typenames: CERT_EXTENSIONS, *PCERT_EXTENSIONS
req.redist: 
---

# CERT_EXTENSIONS structure


## -description


The <b>CERT_EXTENSIONS</b> structure contains an array of extensions.


## -struct-fields




### -field cExtension

Number of elements in the array <b>rgExtension</b>.


### -field rgExtension

Array of structures, each holding information of type <a href="https://msdn.microsoft.com/787a4df0-c0e3-46b9-a7e6-eb3bee3ed717">CERT_EXTENSION</a> about a <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate</a> or <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">CRL</a>.


## -see-also




<a href="https://msdn.microsoft.com/787a4df0-c0e3-46b9-a7e6-eb3bee3ed717">CERT_EXTENSION</a>
 

 

