---
UID: NS:iketypes.IKEEXT_PRESHARED_KEY_AUTHENTICATION0__
title: IKEEXT_PRESHARED_KEY_AUTHENTICATION0
author: windows-sdk-content
description: Stores information needed for pre-shared key authentication.
old-location: fwp\ikeext_preshared_key_authentication0.htm
tech.root: fwp
ms.assetid: 44cd2a76-cd8a-4c52-af41-927b13862c1e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IKEEXT_PRESHARED_KEY_AUTHENTICATION0, IKEEXT_PRESHARED_KEY_AUTHENTICATION0 structure [Filtering], fwp.ikeext_preshared_key_authentication0, iketypes/IKEEXT_PRESHARED_KEY_AUTHENTICATION0
ms.topic: struct
req.header: iketypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Iketypes.idl
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
 - Iketypes.h
api_name:
 - IKEEXT_PRESHARED_KEY_AUTHENTICATION0
product: Windows
targetos: Windows
req.typenames: IKEEXT_PRESHARED_KEY_AUTHENTICATION0
req.redist: 
---

# IKEEXT_PRESHARED_KEY_AUTHENTICATION0 structure


## -description


The <b>IKEEXT_PRESHARED_KEY_AUTHENTICATION0</b> structure stores information needed for pre-shared key authentication.
<div class="alert"><b>Note</b>  <b>IKEEXT_PRESHARED_KEY_AUTHENTICATION0</b> is the specific implementation of IKEEXT_PRESHARED_KEY_AUTHENTICATION used in Windows Vista. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 7 and later, <a href="https://msdn.microsoft.com/b2009797-f5fd-4d14-8a59-832f9a0acff1">IKEEXT_PRESHARED_KEY_AUTHENTICATION1</a> is available.</div><div> </div>

## -struct-fields




### -field presharedKey

The pre-shared key specified by <a href="https://msdn.microsoft.com/85f360bf-5ee4-4980-b4ce-15ff310d8fbe">FWP_BYTE_BLOB</a>.


## -see-also




<a href="https://msdn.microsoft.com/85f360bf-5ee4-4980-b4ce-15ff310d8fbe">FWP_BYTE_BLOB</a>



<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 

