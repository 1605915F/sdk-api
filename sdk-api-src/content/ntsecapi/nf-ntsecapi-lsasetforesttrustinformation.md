---
UID: NF:ntsecapi.LsaSetForestTrustInformation
title: LsaSetForestTrustInformation function
author: windows-sdk-content
description: Sets the forest trust information for a specified Local Security Authority&#160;TrustedDomain object.
old-location: security\lsasetforesttrustinformation.htm
tech.root: secauthn
ms.assetid: 8b0f90ed-7dd4-4803-97c6-31d191b6d2b3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: LsaSetForestTrustInformation, LsaSetForestTrustInformation function [Security], ntsecapi/LsaSetForestTrustInformation, security.lsasetforesttrustinformation
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: ntsecapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.lib: Advapi32.lib
req.dll: Advapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Advapi32.dll
api_name:
 - LsaSetForestTrustInformation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# LsaSetForestTrustInformation function


## -description


The <b>LsaSetForestTrustInformation</b> function sets the forest trust information for a specified <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">Local Security Authority</a> <a href="https://msdn.microsoft.com/fab69367-2143-49ef-a1b9-9c1d846fd4e1">TrustedDomain</a> object.


## -parameters




### -param PolicyHandle [in]

A handle to the <a href="https://msdn.microsoft.com/4253c7fb-85f5-441d-90bf-492e802ad0f8">Policy</a> object for the system.


### -param TrustedDomainName [in]

Pointer to an <a href="https://msdn.microsoft.com/9e1cf20f-01f9-4813-bf95-e47c5d57dcdc">LSA_UNICODE_STRING</a> structure that contains the name of the <a href="https://msdn.microsoft.com/fab69367-2143-49ef-a1b9-9c1d846fd4e1">TrustedDomain</a> object to which to set the forest trust information specified by the <i>ForestTrustInfo</i> parameter.


### -param ForestTrustInfo [in]

Pointer to an <a href="https://msdn.microsoft.com/9e456462-59a9-4f18-ba47-92fc2350889b">LSA_FOREST_TRUST_INFORMATION</a> structure that contains the forest trust information to set to the <a href="https://msdn.microsoft.com/fab69367-2143-49ef-a1b9-9c1d846fd4e1">TrustedDomain</a> object specified by the <i>TrustedDomainName</i> parameter.


### -param CheckOnly [in]

Boolean value that specifies whether changes to the <a href="https://msdn.microsoft.com/fab69367-2143-49ef-a1b9-9c1d846fd4e1">TrustedDomain</a> object are persisted. If this value is <b>TRUE</b>, this function will check for collisions with the specified parameters but will not set the  forest trust information specified by the <i>ForestTrustInfo</i> parameter to the <b>TrustedDomain</b> object specified by the <i>TrustedDomainName</i> parameter. If this value is <b>FALSE</b>, the forest trust information will be set to the  <b>TrustedDomain</b> object.


### -param CollisionInfo [out]

Pointer to a pointer to an <a href="https://msdn.microsoft.com/a4a3b040-c074-4756-a30f-408d8bca87ba">LSA_FOREST_TRUST_COLLISION_INFORMATION</a> structure that returns information about any collisions that occurred.


## -returns



If the function succeeds, the return value is STATUS_SUCCESS.

If the function fails, the return value is an NTSTATUS code, which can be one of the following values or one of the <a href="https://msdn.microsoft.com/ee55364e-8ffe-4a78-a49a-250756561770">LSA Policy Function Return Values</a>.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_INVALID_DOMAIN_STATE</b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The operation is legal only on domain
                                    controllers in the root domain.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_INVALID_DOMAIN_ROLE</b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The operation is legal only on the primary
                                    domain controller.

</td>
</tr>
</table>
 



