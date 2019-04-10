---
UID: NN:comcat.IEnumGUID
title: IEnumGUID (comcat.h)
author: windows-sdk-content
description: Enables clients to enumerate through a collection of class IDs for COM classes.
old-location: com\ienumguid.htm
tech.root: com
ms.assetid: 4f2e0f96-a471-4883-be41-d93806461020
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IEnumGUID, IEnumGUID interface [COM], IEnumGUID interface [COM],described, _com_ienumguid, com.ienumguid, comcat/IEnumGUID
ms.topic: interface
req.header: comcat.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ComCat.idl
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
 - ComCat.h
api_name:
 - IEnumGUID
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumGUID interface


## -description


Enables clients to enumerate through a collection of class IDs for COM classes.



## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumGUID</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IEnumGUID</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumGUID</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5b12adf2-c2fe-4499-ab2a-94af6337e4a2">Clone</a>
</td>
<td align="left" width="63%">
Creates a new enumerator that contains the same enumeration state as the current one.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d32e02c7-1109-40cc-bf36-d224fa59fe20">Next</a>
</td>
<td align="left" width="63%">
Retrieves the specified number of items in the enumeration sequence.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5f31c45a-c7a2-4cdc-a468-76a31a9ba1e9">Reset</a>
</td>
<td align="left" width="63%">
Resets the enumeration sequence to the beginning.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/8c3b955b-ba36-4bab-af89-fc89e08e6e94">Skip</a>
</td>
<td align="left" width="63%">
Skips over the specified number of items in the enumeration sequence.

</td>
</tr>
</table> 


## -remarks



Alternate names for this interface are <a href="https://msdn.microsoft.com/0b2a39e4-105e-4ba7-bfa4-3ecd75dae4b3">IEnumCLSID</a> and <a href="https://msdn.microsoft.com/5255b8a8-6e90-4af0-a086-37b474c644ad">IEnumCATID</a>.



