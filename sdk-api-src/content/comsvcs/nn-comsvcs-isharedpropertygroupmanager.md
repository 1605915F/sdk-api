---
UID: NN:comsvcs.ISharedPropertyGroupManager
title: ISharedPropertyGroupManager (comsvcs.h)
author: windows-sdk-content
description: Used to create shared property groups and to obtain access to existing shared property groups.
old-location: cos\isharedpropertygroupmanager.htm
tech.root: cossdk
ms.assetid: 71c0a1de-5ea5-4496-b0e9-56d0cc8129a9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ISharedPropertyGroupManager, ISharedPropertyGroupManager interface [COM+], ISharedPropertyGroupManager interface [COM+],described, _cos_ISharedPropertyGroupManager, comsvcs/ISharedPropertyGroupManager, cos.isharedpropertygroupmanager
ms.topic: interface
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - ComSvcs.h
api_name:
 - ISharedPropertyGroupManager
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISharedPropertyGroupManager interface


## -description


Used to create shared property groups and to obtain access to existing shared property groups.



## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ISharedPropertyGroupManager</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>ISharedPropertyGroupManager</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ISharedPropertyGroupManager</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/19c954cb-1a3b-4063-a09b-54906ae1613d">CreatePropertyGroup</a>
</td>
<td align="left" width="63%">
Creates a new shared property group.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/04e591c0-6bf4-4864-aaae-57ffd97c5414">get__NewEnum</a>
</td>
<td align="left" width="63%">
Retrieves an enumerator for the named security call context properties.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3e60d1c6-1d58-403a-b75f-2a6bea91081e">get_Group</a>
</td>
<td align="left" width="63%">
Retrieves a reference to an existing shared property group.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/d3c3e888-fe08-4ea6-b94c-fdfcbe7fd08a">ISharedProperty</a>



<a href="https://msdn.microsoft.com/e7f23c83-40d3-4b08-a185-cd6e3260e0a9">ISharedPropertyGroup</a>
 

 

