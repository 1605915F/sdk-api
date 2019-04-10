---
UID: NF:clfsmgmtw32.QueryLogPolicy
title: QueryLogPolicy function (clfsmgmtw32.h)
author: windows-sdk-content
description: The QueryLogPolicy function allows you to obtain a policy that is installed for the specified log.
old-location: fs\querylogpolicy.htm
tech.root: Clfs
ms.assetid: 45bed7c7-132e-48f9-8b9a-d8cb1580f456
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: QueryLogPolicy, QueryLogPolicy function [Files], clfsmgmtw32/QueryLogPolicy, fs.querylogpolicy
ms.topic: function
req.header: clfsmgmtw32.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Clfsw32.lib
req.dll: Clfsw32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Clfsw32.dll
api_name:
 - QueryLogPolicy
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# QueryLogPolicy function


## -description


The <b>QueryLogPolicy</b> function allows you to obtain a policy that is installed for the specified log.


## -parameters




### -param hLog [in]

The handle to the log to query.


### -param ePolicyType [in]

Specifies the type of policy to query for. Policy types are enumerated in <a href="https://msdn.microsoft.com/eaa817be-04ac-48c2-b7de-60509b1f65c7">CLFS_MGMT_POLICY_TYPE</a>.


### -param pPolicyBuffer [out]

A pointer to a buffer to receive the returned policies.


### -param pcbPolicyBuffer [in, out]

A pointer to the size of <i>pPolicyBuffer</i>. If the buffer is not large enough, <i>pcbPolicyBuffer</i> receives the size buffer required to successfully retrieve the specified policies.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero (0). To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -see-also




<a href="https://msdn.microsoft.com/3f5d9c38-b299-4102-9786-115ece5b0928">CLFS_MGMT_POLICY</a>



<a href="https://msdn.microsoft.com/eaa817be-04ac-48c2-b7de-60509b1f65c7">CLFS_MGMT_POLICY_TYPE</a>



<a href="https://msdn.microsoft.com/06e8c1bf-f190-4f3d-a588-5c8dd2e99f43">RemoveLogPolicy</a>
 

 

