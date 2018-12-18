---
UID: NN:wmp.IWMPSettings2
title: IWMPSettings2
author: windows-sdk-content
description: The IWMPSettings2 interface provides methods that supplement the IWMPSettings interface.
old-location: wmp\iwmpsettings2.htm
tech.root: WMP
ms.assetid: 0fb0c7be-015e-4081-8467-c382e0858195
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPSettings2, IWMPSettings2 interface [Windows Media Player], IWMPSettings2 interface [Windows Media Player],described, IWMPSettings2Interface, wmp.iwmpsettings2, wmp/IWMPSettings2
ms.topic: interface
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmp.h
api_name:
 - IWMPSettings2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPSettings2 interface


## -description



The <b>IWMPSettings2</b> interface provides methods that supplement the <b>IWMPSettings</b> interface.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMPSettings2</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Dd563648(v=VS.85).aspx">IWMPSettings</a>. <b>IWMPSettings2</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMPSettings2</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd563650(v=VS.85).aspx">get_defaultAudioLanguage</a>
</td>
<td align="left" width="63%">
Retrieves the locale identifier (LCID) of the default audio language.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd563651(v=VS.85).aspx">get_mediaAccessRights</a>
</td>
<td align="left" width="63%">
Retrieves a value indicating the permissions currently granted for library access.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd563652(v=VS.85).aspx">requestMediaAccessRights</a>
</td>
<td align="left" width="63%">
Requests a specified level of access to the library.

</td>
</tr>
</table> 

Retrieve a pointer to an <b>IWMPSettings2</b> interface by calling the <b>QueryInterface</b> method of the <a href="https://msdn.microsoft.com/en-us/library/Dd563648(v=VS.85).aspx">IWMPSettings</a> interface.

	


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd563648(v=VS.85).aspx">IWMPSettings Interface</a>



<a href="https://msdn.microsoft.com/68a0bdaf-ae1b-4ba1-817b-a31c68b9fddd">Interfaces</a>
 

 

