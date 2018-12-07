---
UID: NF:dhcpsapi.DhcpHlprIsV4PolicyWellFormed
title: DhcpHlprIsV4PolicyWellFormed function
author: windows-sdk-content
description: Verifies that a DHCP server policy structure is well formed.
old-location: dhcp\dhcphlprisv4policywellformed.htm
tech.root: DHCP
ms.assetid: 820b45f6-aa09-4e15-bf77-caa2723f4ea8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DhcpHlprIsV4PolicyWellFormed, DhcpHlprIsV4PolicyWellFormed function [DHCP], dhcp.dhcphlprisv4policywellformed, dhcpsapi/DhcpHlprIsV4PolicyWellFormed
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dhcpsapi.lib
req.dll: Dhcpsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dhcpsapi.dll
api_name:
 - DhcpHlprIsV4PolicyWellFormed
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DhcpHlprIsV4PolicyWellFormed function


## -description


The <b>DhcpHlprIsV4PolicyWellFormed</b> function verifies that a DHCP server policy structure is well formed.


## -parameters




### -param pPolicy [in]

Pointer to <a href="https://msdn.microsoft.com/7e62d2f3-275a-45ab-baab-648fe135d0fc">DHCP_POLICY</a> structure that contains the policy to verify


## -returns



The API returns <b>TRUE</b> if the specified policy satisfies the conditions in the <b>Remarks</b> below. Otherwise, it returns <b>FALSE</b>.




## -remarks



The API performs the following validations on the policy conditions and expression structure.


<ol>
<li>Every clause in the policy condition must have a valid parent expression.</li>
<li>Every expression in the policy structure must have conditions or other expressions as children.</li>
<li>Only one expression must be the root expression.</li>
<li>All non-root expressions must have valid parent expression.</li>
<li>There must be no cyclic relationship between the expressions. Each expression must have the parent expression index lesser than that of itself.</li>
</ol>



## -see-also




<a href="https://msdn.microsoft.com/7c90625c-e6b5-475f-a9ea-0dfd27810f03">DhcpHlprAddV4PolicyCondition</a>



<a href="https://msdn.microsoft.com/549d86ed-81c1-4126-9f43-f7e5340990d3">DhcpHlprAddV4PolicyExpr</a>



<a href="https://msdn.microsoft.com/4e5b5fca-7583-43a8-8816-c1003d936233">DhcpHlprAddV4PolicyRange</a>



<a href="https://msdn.microsoft.com/91f04578-9f15-44b4-8cf6-99be13d0395e">DhcpHlprCreateV4Policy</a>



<a href="https://msdn.microsoft.com/ace10974-784b-41f7-aee9-461c8d63b479">DhcpHlprFreeV4Policy</a>



<a href="https://msdn.microsoft.com/46c20727-0e7a-42cf-a571-c1198b124ed0">DhcpHlprIsV4PolicySingleUC</a>



<a href="https://msdn.microsoft.com/f11386a6-2b80-4a2b-b859-fb399d7392e8">DhcpHlprIsV4PolicyValid</a>



<a href="https://msdn.microsoft.com/5d6818f9-4e44-4f24-a489-84defd1117c0">DhcpHlprModifyV4PolicyExpr</a>



<a href="https://msdn.microsoft.com/5f252840-d474-405e-8b32-50e6efe35f62">DhcpHlprResetV4PolicyExpr</a>
 

 

