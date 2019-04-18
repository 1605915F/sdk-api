---
UID: NF:azroles.IAzBizRuleParameters.AddParameters
title: IAzBizRuleParameters::AddParameters (azroles.h)
author: windows-sdk-content
description: Adds parameters to the list of parameters available to business rule (BizRule) scripts.
old-location: security\iazbizruleparameters_addparameters_method.htm
tech.root: SecAuthZ
ms.assetid: ebf336a9-a64a-4ded-b508-56491ebf48e2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: AddParameters, AddParameters method [Security], AddParameters method [Security],IAzBizRuleParameters interface, IAzBizRuleParameters interface [Security],AddParameters method, IAzBizRuleParameters.AddParameters, IAzBizRuleParameters::AddParameters, azroles/IAzBizRuleParameters::AddParameters, security.iazbizruleparameters_addparameters_method
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
 - IAzBizRuleParameters.AddParameters
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAzBizRuleParameters::AddParameters


## -description


The <b>AddParameters</b> method adds  parameters to the list of parameters available to business rule (BizRule) scripts.


## -parameters




### -param varParameterNames [in]

The parameter names. This is a variant that contains either a <a href="https://msdn.microsoft.com/en-us/library/ms221482(v=VS.85).aspx">SAFEARRAY</a> or the  JScript <a href="https://msdn.microsoft.com/library/k4h76zbx(v=VS.85).aspx">Array</a> object. Each element of the array holds a <b>VT_BSTR</b> that contains a parameter name. This array must be sorted alphabetically; the sort order is as defined by a case-sensitive <a href="https://msdn.microsoft.com/en-us/library/ms221006(v=VS.85).aspx">VarCmp</a>. The order of the <i>varParameterValues</i> array must match the order of this array. 


### -param varParameterValues [in]

The values of the parameters that are available to BizRule scripts. This is a variant that contains either a <a href="https://msdn.microsoft.com/en-us/library/ms221482(v=VS.85).aspx">SAFEARRAY</a> or the  JScript <a href="https://msdn.microsoft.com/library/k4h76zbx(v=VS.85).aspx">Array</a> object. Each element of the array holds a value that corresponds to an element in the <i>varParameterNames</i> array. The default value is <b>VT_NULL</b>. The entries in the array can hold any type except <b>VT_UNKNOWN</b> and <b>VT_DISPATCH</b>.


## -returns



 If the method succeeds, it returns <b>S_OK</b>.

If the method fails, it returns an error code. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.




## -see-also




<a href="https://msdn.microsoft.com/07eb33be-71a3-42fc-b7f3-12be23746aa3">IAzBizRuleParameters</a>



<a href="https://msdn.microsoft.com/161f8a84-ee00-4f39-9997-a1e3d1c5b7a8">IAzClientContext3::BizRuleParameters</a>
 

 

