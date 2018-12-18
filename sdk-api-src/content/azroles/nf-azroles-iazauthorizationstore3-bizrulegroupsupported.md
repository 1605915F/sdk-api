---
UID: NF:azroles.IAzAuthorizationStore3.BizruleGroupSupported
title: IAzAuthorizationStore3::BizruleGroupSupported
author: windows-sdk-content
description: Returns a Boolean value that specifies whether this IAzAuthorizationStore3 object supports application groups that use business rule (BizRule) scripts.
old-location: security\iazauthorizationstore3_bizrulegroupsupported_method.htm
tech.root: secauthz
ms.assetid: 88449b12-5086-4f86-94d4-2a4afb4be070
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BizruleGroupSupported, BizruleGroupSupported method [Security], BizruleGroupSupported method [Security],IAzAuthorizationStore3 interface, IAzAuthorizationStore3 interface [Security],BizruleGroupSupported method, IAzAuthorizationStore3.BizruleGroupSupported, IAzAuthorizationStore3::BizruleGroupSupported, azroles/IAzAuthorizationStore3::BizruleGroupSupported, security.iazauthorizationstore3_bizrulegroupsupported_method
ms.topic: method
req.header: azroles.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Azroles.idl
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
 - COM
api_location:
 - Azroles.h
api_name:
 - IAzAuthorizationStore3.BizruleGroupSupported
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAzAuthorizationStore3::BizruleGroupSupported


## -description


The <b>BizruleGroupSupported</b> method returns a Boolean value that specifies whether this <a href="https://msdn.microsoft.com/7063416c-b132-4b3a-bb2b-d27fccea25e4">IAzAuthorizationStore3</a> object supports application groups that use business rule (BizRule) scripts.


## -parameters




### -param pbSupported [out]

<b>VARIANT_TRUE</b> if the current <a href="https://msdn.microsoft.com/7063416c-b132-4b3a-bb2b-d27fccea25e4">IAzAuthorizationStore3</a> object supports scripts that use business logic to determine group membership; otherwise, <b>VARIANT_FALSE</b>.


## -returns



 If the method succeeds, it returns <b>S_OK</b>.

If the method fails, it returns an error code. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.



