---
UID: NS:iketypes.IKEEXT_EM_POLICY0_
title: IKEEXT_EM_POLICY0 (iketypes.h)
author: windows-sdk-content
description: Is used to store AuthIP's extended mode negotiation policy.
old-location: fwp\ikeext_em_policy0.htm
tech.root: fwp
ms.assetid: 954a2bb8-eb54-4f41-8a0c-3f2af1190f57
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IKEEXT_EM_POLICY0, IKEEXT_EM_POLICY0 structure [Filtering], fwp.ikeext_em_policy0, iketypes/IKEEXT_EM_POLICY0
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
 - IKEEXT_EM_POLICY0
product: Windows
targetos: Windows
req.typenames: IKEEXT_EM_POLICY0
req.redist: 
---

# IKEEXT_EM_POLICY0 structure


## -description


The <b>IKEEXT_EM_POLICY0</b> structure is used to store AuthIP's extended mode negotiation policy.
<div class="alert"><b>Note</b>  <b>IKEEXT_EM_POLICY0</b> is the specific implementation of IKEEXT_EM_POLICY used in Windows Vista. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 7, <a href="https://msdn.microsoft.com/dae56d71-31e0-4746-8bfb-4ade3705278f">IKEEXT_EM_POLICY1</a> is available.  For Windows 8, <a href="https://msdn.microsoft.com/01e3122b-812f-4c01-a514-dc0d513de822">IKEEXT_EM_POLICY2</a> is available.</div><div> </div>

## -struct-fields




### -field numAuthenticationMethods

Number of authentication methods in the array.


### -field authenticationMethods

size_is(numAuthenticationMethods)

Array of acceptable authentication methods as specified by <a href="https://msdn.microsoft.com/ce11d9ac-2636-432b-9bc7-3509f52478d9">IKEEXT_AUTHENTICATION_METHOD0</a>.


### -field initiatorImpersonationType

Type of impersonation.

See <a href="https://msdn.microsoft.com/en-us/library/Aa364974(v=VS.85).aspx">IKEEXT_AUTHENTICATION_IMPERSONATION_TYPE</a> for more information.


## -remarks



Applies only to AuthIP.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa364974(v=VS.85).aspx">IKEEXT_AUTHENTICATION_IMPERSONATION_TYPE</a>



<a href="https://msdn.microsoft.com/ce11d9ac-2636-432b-9bc7-3509f52478d9">IKEEXT_AUTHENTICATION_METHOD0</a>



<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 

