---
UID: NF:propsys.IPropertyDescription.GetViewFlags
title: IPropertyDescription::GetViewFlags (propsys.h)
author: windows-sdk-content
description: Gets the current set of flags governing the property's view.
old-location: properties\IPropertyDescription_GetViewFlags.htm
tech.root: properties
ms.assetid: 73b60861-3d73-4bff-ae46-a7683d708c83
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetViewFlags, GetViewFlags method [Windows Properties], GetViewFlags method [Windows Properties],IPropertyDescription interface, IPropertyDescription interface [Windows Properties],GetViewFlags method, IPropertyDescription.GetViewFlags, IPropertyDescription::GetViewFlags, properties.IPropertyDescription_GetViewFlags, propsys/IPropertyDescription::GetViewFlags, shell.IPropertyDescription_GetViewFlags, shell_IPropertyDescription_GetViewFlags
ms.topic: method
f1_keywords: ["propsys/IPropertyDescription.GetViewFlags"]
req.header: propsys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Propsys.idl
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
 - Propsys.h
api_name:
 - IPropertyDescription.GetViewFlags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPropertyDescription::GetViewFlags


## -description


Gets the current set of flags governing the property's view.


## -parameters




### -param ppdvFlags [out]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/propsys/ne-propsys-propdesc_view_flags">PROPDESC_VIEW_FLAGS</a>*</b>

When this method returns, contains a pointer to a value that includes one or more of the following flags. See <a href="https://docs.microsoft.com/windows/desktop/api/propsys/ne-propsys-propdesc_view_flags">PROPDESC_VIEW_FLAGS</a> for valid values.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/propsys/nn-propsys-ipropertydescription">IPropertyDescription</a>



<a href="https://docs.microsoft.com/windows/desktop/properties/propdesc-schema-entry">Property Description Schema</a>
 

 

