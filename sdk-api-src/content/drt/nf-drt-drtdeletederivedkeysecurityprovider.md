---
UID: NF:drt.DrtDeleteDerivedKeySecurityProvider
title: DrtDeleteDerivedKeySecurityProvider function (drt.h)
author: windows-sdk-content
description: DrtDeleteDerivedKeySecurityProvider function deletes a derived key security provider for a Distributed Routing Table.
old-location: p2p\drtdeletederivedkeysecurityprovider.htm
tech.root: P2PSdk
ms.assetid: 89b2bbe6-51a3-48fc-85c9-13e1b0cfd880
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DrtDeleteDerivedKeySecurityProvider, DrtDeleteDerivedKeySecurityProvider function [Peer Networking], drt/DrtDeleteDerivedKeySecurityProvider, p2p.drtdeletederivedkeysecurityprovider
ms.topic: function
req.header: drt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 Professional [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Drtprov.lib
req.dll: Drt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - drt.dll
api_name:
 - DrtDeleteDerivedKeySecurityProvider
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DrtDeleteDerivedKeySecurityProvider function


## -description


The <b>DrtDeleteDerivedKeySecurityProvider</b> function deletes a derived key security provider for a Distributed Routing Table.


## -parameters




### -param pSecurityProvider [in]

Pointer to a <a href="https://msdn.microsoft.com/1eedfff3-d561-462e-bad0-45e7bc46fb1a">DRT_SECURITY_PROVIDER</a> specifying the security provider to delete.


## -returns



This function does not return a value.




## -see-also




<a href="https://msdn.microsoft.com/069358e0-4b61-44ed-b235-37f1d038feff">DrtCreateDerivedKey</a>



<a href="https://msdn.microsoft.com/e4cc8326-e2bc-459f-97dd-a00cfd1ed35e">DrtCreateDerivedKeySecurityProvider</a>
 

 

