---
UID: NF:azroles.IAzTask.get_BizRule
title: IAzTask::get_BizRule
author: windows-sdk-content
description: Sets or retrieves the text of the script that implements the business rule (BizRule).
old-location: security\iaztask_bizrule.htm
tech.root: secauthz
ms.assetid: cf3d87af-5320-4fe0-b513-e242f8a1dd1b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzTask object [Security],BizRule property, BizRule property [Security], BizRule property [Security],AzTask object, BizRule property [Security],IAzTask interface, IAzTask interface [Security],BizRule property, IAzTask.BizRule, IAzTask.get_BizRule, IAzTask::BizRule, IAzTask::get_BizRule, IAzTask::put_BizRule, azroles/IAzTask::BizRule, azroles/IAzTask::get_BizRule, azroles/IAzTask::put_BizRule, get_BizRule, security.iaztask_bizrule
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: azroles.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: Azroles.lib
req.dll: Azroles.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Azroles.dll
api_name:
 - IAzTask.BizRule
 - IAzTask.get_BizRule
 - IAzTask.put_BizRule
 - AzTask.BizRule
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzTask::get_BizRule


## -description


The <b>BizRule</b> property sets or retrieves the text of the script that implements the business rule (BizRule).

This property is read/write.


## -parameters


## -remarks



The maximum length of this property is 65,536 characters.

<div class="alert"><b>Important</b>  The <a href="https://msdn.microsoft.com/en-us/library/Aa378380(v=VS.85).aspx">BizRuleLanguage</a> property must be set before this property is set.</div>
<div> </div>
An <a href="https://msdn.microsoft.com/en-us/library/Aa378367(v=VS.85).aspx">IAzTask</a> object that is a child object of a delegated <a href="https://msdn.microsoft.com/en-us/library/Aa378237(v=VS.85).aspx">IAzScope</a> object cannot have an associated BizRule.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa378379(v=VS.85).aspx">BizRuleImportedPath</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa378380(v=VS.85).aspx">BizRuleLanguage</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa378367(v=VS.85).aspx">IAzTask</a>
 

 

