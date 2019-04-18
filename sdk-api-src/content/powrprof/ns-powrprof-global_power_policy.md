---
UID: NS:powrprof._GLOBAL_POWER_POLICY
title: GLOBAL_POWER_POLICY (powrprof.h)
author: windows-sdk-content
description: Contains global power policy settings that apply to all power schemes.
old-location: base\global_power_policy_str.htm
tech.root: power
ms.assetid: 5c177093-0c16-4a84-9212-f2376de6965b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PGLOBAL_POWER_POLICY, GLOBAL_POWER_POLICY, GLOBAL_POWER_POLICY structure, PGLOBAL_POWER_POLICY, PGLOBAL_POWER_POLICY structure pointer, _win32_global_power_policy_str, base.global_power_policy_str, powrprof/GLOBAL_POWER_POLICY, powrprof/PGLOBAL_POWER_POLICY"
ms.topic: struct
req.header: powrprof.h
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
 - PowrProf.h
api_name:
 - GLOBAL_POWER_POLICY
product: Windows
targetos: Windows
req.typenames: GLOBAL_POWER_POLICY, *PGLOBAL_POWER_POLICY
req.redist: 
ms.custom: 19H1
---

# GLOBAL_POWER_POLICY structure


## -description


Contains global power policy settings that apply to all power schemes.


## -struct-fields




### -field user

A 
<a href="https://msdn.microsoft.com/0e89ae66-a889-4929-b028-125fcef5c89c">GLOBAL_USER_POWER_POLICY</a> structure that defines the global user power policy settings.


### -field mach

A 
<a href="https://msdn.microsoft.com/79b57da4-0125-427b-aec7-7ca4c9bfb870">GLOBAL_MACHINE_POWER_POLICY</a> structure that defines the global computer power policy settings.


## -see-also




<a href="https://msdn.microsoft.com/79b57da4-0125-427b-aec7-7ca4c9bfb870">GLOBAL_MACHINE_POWER_POLICY</a>



<a href="https://msdn.microsoft.com/0e89ae66-a889-4929-b028-125fcef5c89c">GLOBAL_USER_POWER_POLICY</a>



<a href="https://msdn.microsoft.com/9a834fb6-35ae-4d36-885c-0d81cd39e9a6">GetCurrentPowerPolicies</a>



<a href="https://msdn.microsoft.com/65da3d9f-b688-4d41-9da0-05159297d169">ReadGlobalPwrPolicy</a>



<a href="https://msdn.microsoft.com/f449ff0d-5c22-4c6d-8c88-dc18258a8c6d">SetActivePwrScheme</a>



<a href="https://msdn.microsoft.com/293dc3a5-5e6b-4709-8439-67d2339740e7">WriteGlobalPwrPolicy</a>
 

 

