---
UID: NN:bits4_0.IBitsTokenOptions
title: IBitsTokenOptions
author: windows-sdk-content
description: Use IBitsTokenOptions to associate and manage a pair of security tokens for a Background Intelligent Transfer Service (BITS) transfer job.
old-location: bits\ibitstokenoptions.htm
tech.root: bits
ms.assetid: 8496c27b-68d8-4709-b8a6-6ffa17c886df
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBitsTokenOptions, IBitsTokenOptions interface [BITS], IBitsTokenOptions interface [BITS],described, bits.ibitstokenoptions, bits4_0/IBitsTokenOptions
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: bits4_0.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits4_0.idl
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
 - Bits4_0.h
api_name:
 - IBitsTokenOptions
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Management Framework on  Windows Vista with SP1,  Windows Vista with SP2, and  Windows Server 2008 with SP2
---

# IBitsTokenOptions interface


## -description


Use <b>IBitsTokenOptions</b> to associate and manage a pair of security tokens for a Background Intelligent Transfer Service (BITS) transfer job.

To get this interface, call the <a href="https://msdn.microsoft.com/en-us/library/Aa362973(v=VS.85).aspx">IBackgroundCopyJob::QueryInterface</a> method, using __uuidof(IBitsTokenOptions) as the interface identifier.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IBitsTokenOptions</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IBitsTokenOptions</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>IBitsTokenOptions</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd904471(v=VS.85).aspx">ClearHelperToken</a>
</td>
<td align="left" width="63%">
Discards the helper token and does not change the usage flags.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd904472(v=VS.85).aspx">GetHelperTokenFlags</a>
</td>
<td align="left" width="63%">
Returns the usage flags for a token that is associated with a BITS transfer job.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd904473(v=VS.85).aspx">GetHelperTokenSid</a>
</td>
<td align="left" width="63%">
Returns the SID of the helper token if one is set.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd904474(v=VS.85).aspx">SetHelperToken</a>
</td>
<td align="left" width="63%">
Sets the helper token to impersonate the token of the COM client.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd904475(v=VS.85).aspx">SetHelperTokenFlags</a>
</td>
<td align="left" width="63%">
Sets the usage flags for a token that is associated with a BITS transfer job.

</td>
</tr>
</table> 

