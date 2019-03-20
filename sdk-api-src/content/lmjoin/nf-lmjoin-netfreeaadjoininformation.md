---
UID: NF:lmjoin.NetFreeAadJoinInformation
title: NetFreeAadJoinInformation function (lmjoin.h)
author: windows-sdk-content
description: Frees the memory allocated for the specified DSREG_JOIN_INFO structure, which contains join information for a tenant and which you retrieved by calling the NetGetAadJoinInformation function.
old-location: netmgmt\netfreeaadjoininformation.htm
tech.root: NetMgmt
ms.assetid: BDFB6179-4B8C-43E3-8D34-A2B470EA0D0B
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: NetFreeAadJoinInformation, NetFreeAadJoinInformation function [Network Management], lmjoin/NetFreeAadJoinInformation, netmgmt.netfreeaadjoininformation
ms.topic: function
req.header: lmjoin.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Netapi32.lib
req.dll: Netapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - netapi32.dll
api_name:
 - NetFreeAadJoinInformation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# NetFreeAadJoinInformation function


## -description


Frees the memory allocated for the specified <a href="https://msdn.microsoft.com/9B0F7BE3-BDCD-437E-9157-9A646A2A20E2">DSREG_JOIN_INFO</a> structure, which contains join information for a tenant and which you retrieved by calling the <a href="https://msdn.microsoft.com/C63B3AA7-FC7E-4CB9-9318-BD25560591AB">NetGetAadJoinInformation</a> function.


## -parameters




### -param pJoinInfo [in, optional]

Pointer to the <a href="https://msdn.microsoft.com/9B0F7BE3-BDCD-437E-9157-9A646A2A20E2">DSREG_JOIN_INFO</a> structure for which you want to free the memory. 


## -returns



This function does not return a value.




## -see-also




<a href="https://msdn.microsoft.com/9B0F7BE3-BDCD-437E-9157-9A646A2A20E2">DSREG_JOIN_INFO</a>



<a href="https://msdn.microsoft.com/C63B3AA7-FC7E-4CB9-9318-BD25560591AB">NetGetAadJoinInformation</a>
 

 

