---
UID: NF:propsys.IPropertyDescription.GetCanonicalName
title: IPropertyDescription::GetCanonicalName
author: windows-sdk-content
description: Gets the case-sensitive name by which a property is known to the system, regardless of its localized name.
old-location: properties\IPropertyDescription_GetCanonicalName.htm
tech.root: properties
ms.assetid: 861c3b48-77cf-4f72-b85f-a6f921571dd7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCanonicalName, GetCanonicalName method [Windows Properties], GetCanonicalName method [Windows Properties],IPropertyDescription interface, IPropertyDescription interface [Windows Properties],GetCanonicalName method, IPropertyDescription.GetCanonicalName, IPropertyDescription::GetCanonicalName, properties.IPropertyDescription_GetCanonicalName, propsys/IPropertyDescription::GetCanonicalName, shell.IPropertyDescription_GetCanonicalName, shell_IPropertyDescription_GetCanonicalName
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
 - IPropertyDescription.GetCanonicalName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPropertyDescription::GetCanonicalName


## -description


Gets the case-sensitive name by which a property is known to the system, regardless of its localized name.


## -parameters




### -param ppszName [out]

Type: <b>LPWSTR*</b>

When this method returns, contains the address of a pointer to the property's canonical name as a null-terminated Unicode string.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The information retrieved by this method comes from the <i>name</i> attribute of the <a href="shell.propdesc_schema_propertyDescription">propertyDescription</a> element in the property's .propdesc file.

It is the responsibility of the calling application to use <a href="https://msdn.microsoft.com/3d0af12e-fc74-4ef7-b2dd-e9da5d0483c7">CoTaskMemFree</a> to release the string referred to by <i>ppszName</i> when it is no longer needed.
            




## -see-also




<a href="shell.IPropertyDescription">IPropertyDescription</a>



<a href="https://msdn.microsoft.com/cac93c31-d90d-4116-b846-0cf593d1d56e">Property Description Schema</a>
 

 

