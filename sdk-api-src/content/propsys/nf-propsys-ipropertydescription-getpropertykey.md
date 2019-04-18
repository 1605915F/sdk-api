---
UID: NF:propsys.IPropertyDescription.GetPropertyKey
title: IPropertyDescription::GetPropertyKey (propsys.h)
author: windows-sdk-content
description: Gets a structure that acts as a property's unique identifier.
old-location: properties\IPropertyDescription_GetPropertyKey.htm
tech.root: properties
ms.assetid: 10942dff-234e-4f85-827b-f27a6f099818
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetPropertyKey, GetPropertyKey method [Windows Properties], GetPropertyKey method [Windows Properties],IPropertyDescription interface, IPropertyDescription interface [Windows Properties],GetPropertyKey method, IPropertyDescription.GetPropertyKey, IPropertyDescription::GetPropertyKey, properties.IPropertyDescription_GetPropertyKey, propsys/IPropertyDescription::GetPropertyKey, shell.IPropertyDescription_GetPropertyKey, shell_IPropertyDescription_GetPropertyKey
ms.topic: method
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
 - IPropertyDescription.GetPropertyKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPropertyDescription::GetPropertyKey


## -description


Gets a structure that acts as a property's unique identifier.


## -parameters




### -param pkey [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb773381(v=VS.85).aspx">PROPERTYKEY</a>*</b>

When this method returns, contains a pointer to a <a href="https://msdn.microsoft.com/en-us/library/Bb773381(v=VS.85).aspx">PROPERTYKEY</a> structure.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The information retrieved by this method comes from the <a href="https://msdn.microsoft.com/en-us/library/Bb773880(v=VS.85).aspx">propertyDescription</a> element in the property's .propdesc file.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb761561(v=VS.85).aspx">IPropertyDescription</a>



<a href="https://msdn.microsoft.com/cac93c31-d90d-4116-b846-0cf593d1d56e">Property Description Schema</a>
 

 

