---
UID: NF:gpedit.IGroupPolicyObject.GetOptions
title: IGroupPolicyObject::GetOptions (gpedit.h)
author: windows-sdk-content
description: The GetOptions method retrieves the options for the GPO.
old-location: policy\igrouppolicyobject_getoptions.htm
tech.root: Policy
ms.assetid: a4b86196-04c8-4ec1-bf26-2a33e44020d2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GPO_OPTION_DISABLE_MACHINE, GPO_OPTION_DISABLE_USER, GetOptions, GetOptions method [Group Policy], GetOptions method [Group Policy],IGroupPolicyObject interface, IGroupPolicyObject interface [Group Policy],GetOptions method, IGroupPolicyObject.GetOptions, IGroupPolicyObject::GetOptions, _win32_igrouppolicyobject_getoptions, gpedit/IGroupPolicyObject::GetOptions, policy.igrouppolicyobject_getoptions
ms.topic: method
req.header: gpedit.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Gpedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gpedit.dll
api_name:
 - IGroupPolicyObject.GetOptions
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IGroupPolicyObject::GetOptions


## -description


The
    <b>GetOptions</b> method retrieves the options for the GPO.


## -parameters




### -param dwOptions [out]

Receives the options. This parameter can be one or more of the following options.



#### GPO_OPTION_DISABLE_USER

The user portion of the GPO is disabled.



#### GPO_OPTION_DISABLE_MACHINE

The computer portion of the GPO is disabled.


## -returns



If the method succeeds, the return value is <b>S_OK</b>. Otherwise, the method returns one of the COM error codes defined in the Platform SDK header file WinError.h.




## -remarks



To set the options for a GPO, you can call the 
<a href="https://msdn.microsoft.com/4caed430-2861-49cb-9418-b12bf1c46707">SetOptions</a> method.




## -see-also




<a href="https://msdn.microsoft.com/dc15a69d-a44d-4731-a9e5-6165abd581c4">Group Policy
    Interfaces</a>



<a href="https://msdn.microsoft.com/1285ab5a-ea68-4c16-bc34-8ab2f3cfad35">Group Policy
    Overview</a>



<a href="https://msdn.microsoft.com/b3cd31a1-c238-4eb2-8164-9c4891e6227b">IGroupPolicyObject</a>



<a href="https://msdn.microsoft.com/4caed430-2861-49cb-9418-b12bf1c46707">SetOptions</a>
 

 

