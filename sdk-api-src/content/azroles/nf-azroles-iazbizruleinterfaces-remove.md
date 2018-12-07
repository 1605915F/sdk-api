---
UID: NF:azroles.IAzBizRuleInterfaces.Remove
title: IAzBizRuleInterfaces::Remove
author: windows-sdk-content
description: Removes the specified interface from the list of interfaces The number of interfaces in the list of interfaces that can be called by BizRule scripts.
old-location: security\iazbizruleinterfaces_remove_method.htm
tech.root: secauthz
ms.assetid: 398e4151-aeda-48d0-b6f5-e0ea749d0720
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAzBizRuleInterfaces interface [Security],Remove method, IAzBizRuleInterfaces.Remove, IAzBizRuleInterfaces::Remove, Remove, Remove method [Security], Remove method [Security],IAzBizRuleInterfaces interface, azroles/IAzBizRuleInterfaces::Remove, security.iazbizruleinterfaces_remove_method
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IAzBizRuleInterfaces.Remove
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAzBizRuleInterfaces::Remove


## -description


The <b>Remove</b> method removes the specified interface from the list of interfaces The number of interfaces in the list of interfaces that can be called by BizRule scripts.


## -parameters




### -param bstrInterfaceName [in]

The name of the interface to remove.


## -returns



 If the method succeeds, it returns <b>S_OK</b>.

If the method fails, it returns an error code. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa965800(v=VS.85).aspx">AddInterface</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa377614(v=VS.85).aspx">IAzBizRuleInterfaces</a>
 

 

