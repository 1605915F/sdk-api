---
UID: NF:propsys.IPropertyDescription.GetDefaultColumnWidth
title: IPropertyDescription::GetDefaultColumnWidth (propsys.h)
author: windows-sdk-content
description: Gets the default column width of the property in a list view.
old-location: properties\IPropertyDescription_GetDefaultColumnWidth.htm
tech.root: properties
ms.assetid: 3f39cb88-084b-4eca-8168-871dcdc74f98
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDefaultColumnWidth, GetDefaultColumnWidth method [Windows Properties], GetDefaultColumnWidth method [Windows Properties],IPropertyDescription interface, IPropertyDescription interface [Windows Properties],GetDefaultColumnWidth method, IPropertyDescription.GetDefaultColumnWidth, IPropertyDescription::GetDefaultColumnWidth, properties.IPropertyDescription_GetDefaultColumnWidth, propsys/IPropertyDescription::GetDefaultColumnWidth, shell.IPropertyDescription_GetDefaultColumnWidth, shell_IPropertyDescription_GetDefaultColumnWidth
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
 - IPropertyDescription.GetDefaultColumnWidth
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPropertyDescription::GetDefaultColumnWidth


## -description


Gets the default column width of the property in a list view.


## -parameters




### -param pcxChars [out]

Type: <b>DWORD*</b>

A pointer to the column width value, in characters.


## -returns



Type: <b>HRESULT</b>

Always returns <b>S_OK</b>.




## -remarks



The values retrieved by this method are originally set through the <i>defaultColumnWidth</i> attribute of the <a href="https://msdn.microsoft.com/en-us/library/Bb773865(v=VS.85).aspx">displayInfo</a> element in the property's .propdesc file.

If no value is set in the .propdesc file or if the method fails, the value pointed to by <i>pcxChars</i> is 20 characters.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb761561(v=VS.85).aspx">IPropertyDescription</a>



<a href="https://msdn.microsoft.com/cac93c31-d90d-4116-b846-0cf593d1d56e">Property Description Schema</a>
 

 

