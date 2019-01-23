---
UID: NF:wcmconfig.ISettingsItem.GetRestriction
title: ISettingsItem::GetRestriction
author: windows-sdk-content
description: Gets the information for a given restriction.
old-location: smi\isettingsitem_getrestriction.htm
tech.root: SMI
ms.assetid: 14bc4956-e8ea-464b-949e-ddc7ae445c1a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetRestriction, GetRestriction method [SMI], GetRestriction method [SMI],ISettingsItem interface, ISettingsItem interface [SMI],GetRestriction method, ISettingsItem.GetRestriction, ISettingsItem::GetRestriction, smi.isettingsitem_getrestriction, wcmconfig/ISettingsItem::GetRestriction
ms.topic: method
req.header: wcmconfig.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WcmConfig.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: SMIEngine.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - SMIEngine.dll
api_name:
 - ISettingsItem.GetRestriction
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISettingsItem::GetRestriction


## -description


Gets the information for a given restriction.


## -parameters




### -param RestrictionFacet [in]

A <a href="https://msdn.microsoft.com/en-us/library/Aa378606(v=VS.85).aspx">WcmRestrictionFacets</a> value that indicates the type of restriction facet.


### -param FacetData [out]

A pointer to the facet data.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Indicates success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>HRESULT_FROM_WIN32 (ERROR_INVALID_OPERATION)</b></dt>
</dl>
</td>
<td width="60%">
Indicates that the method was called on a non-scalar setting.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Indicates that the requested restriction facet is not defined for this item.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/a743d942-69f9-426b-be88-adf88b9bb1e0">ISettingsItem</a>
 

 

