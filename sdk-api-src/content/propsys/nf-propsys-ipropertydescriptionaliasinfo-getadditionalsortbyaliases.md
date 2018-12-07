---
UID: NF:propsys.IPropertyDescriptionAliasInfo.GetAdditionalSortByAliases
title: IPropertyDescriptionAliasInfo::GetAdditionalSortByAliases
author: windows-sdk-content
description: Gets the address of a pointer to the IPropertyDescriptionList interface, which contains additional sort column values.
old-location: properties\IPropertyDescriptionAliasInfo_GetAdditionalSortByAliases.htm
tech.root: properties
ms.assetid: fb7c105b-6e81-4837-ad00-8886abbe108f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAdditionalSortByAliases, GetAdditionalSortByAliases method [Windows Properties], GetAdditionalSortByAliases method [Windows Properties],IPropertyDescriptionAliasInfo interface, IPropertyDescriptionAliasInfo interface [Windows Properties],GetAdditionalSortByAliases method, IPropertyDescriptionAliasInfo.GetAdditionalSortByAliases, IPropertyDescriptionAliasInfo::GetAdditionalSortByAliases, _shell_IPropertyDescriptionAliasInfo_GetAdditionalSortByAliases, properties.IPropertyDescriptionAliasInfo_GetAdditionalSortByAliases, propsys/IPropertyDescriptionAliasInfo::GetAdditionalSortByAliases, shell.IPropertyDescriptionAliasInfo_GetAdditionalSortByAliases
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IPropertyDescriptionAliasInfo.GetAdditionalSortByAliases
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPropertyDescriptionAliasInfo::GetAdditionalSortByAliases


## -description


Gets the address of a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a> interface, which contains additional sort column values.


## -parameters




### -param riid [in]

Type: <b>REFIID</b>

A reference to the identifier of the requested <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a> interface.


### -param ppv [out]

Type: <b>void**</b>

When this method returns successfully, contains the address of a pointer to an <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a> interface.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The following is an example usage for this method. When sorting by System.Author: System.DateModified, System.DateCreated, and System.ItemNameDisplay may be used as secondary sort columns.  This ensures a unique sort order (for System.Author) and is used to provide a more consistent user experience.


 Calling applications include any UI that wants the secondary sort columns for a given property.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb761517(v=VS.85).aspx">IPropertyDescriptionAliasInfo</a>



<a href="https://msdn.microsoft.com/library/Bb761515(v=VS.85).aspx">IPropertyDescriptionAliasInfo::GetSortByAlias</a>
 

 

