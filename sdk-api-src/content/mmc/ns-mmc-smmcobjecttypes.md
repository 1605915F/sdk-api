---
UID: NS:mmc._SMMCObjectTypes
title: SMMCObjectTypes (mmc.h)
author: windows-sdk-content
description: The SMMCDynamicExtensions structure is introduced in MMC 1.1.
old-location: mmc\smmcdynamicextensions.htm
tech.root: mmc
ms.assetid: 59acd90c-60de-457a-94d7-418b79247a2e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SMMCDynamicExtensions, SMMCDynamicExtensions structure [MMC], SMMCObjectTypes, SMMCObjectTypes structure [MMC], _slate_smmcdynamicextensions, mmc.smmcdynamicextensions, mmc/SMMCDynamicExtensions
ms.topic: struct
req.header: mmc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
 - HeaderDef
api_location:
 - Mmc.h
api_name:
 - SMMCObjectTypes
product: Windows
targetos: Windows
req.typenames: SMMCObjectTypes
req.redist: 
---

# SMMCObjectTypes structure


## -description


The 
<b>SMMCDynamicExtensions</b> structure is introduced in MMC 1.1.

The 
<b>SMMCDynamicExtensions</b> structure defines the format of the data for the 
<a href="https://msdn.microsoft.com/48d55143-7873-4c66-a4c9-bde5663cb7f1">CCF_MMC_DYNAMIC_EXTENSIONS</a> clipboard format, which specifies the non-namespace extension snap-ins that should extend a scope or result item.


## -struct-fields




### -field count

The count of GUIDs in the array specified by <b>guid</b>.


### -field guid

An array of GUIDs that represent the CLSIDs of the snap-ins that you want to extend the item represented by an <b>IDataObject</b> object.


## -remarks



For a snap-in to support dynamic extension of its items with non-namespace extensions (that is, context menu, toolbar, property sheet, or taskpad extensions), the clipboard format CCF_MMC_DYNAMIC_EXTENSIONS must be handled in the snap-in's <b>IDataObject</b> implementation. For more information, see 
<a href="https://msdn.microsoft.com/6087bd8a-08bf-4430-be9e-258262c60900">Dynamic Non-Namespace Extensions</a>.

Be aware that the extension snap-in must be a non-namespace extension and the MMC registry entries for the snap-in to be extended as well as the extension snap-in must be set correctly. For details on setting MMC registry entries for extensions, see 
<a href="https://msdn.microsoft.com/6edbd21d-2ec8-4142-97ec-be089d810b7e">Registration Requirements for Extension Snap-ins</a>.

The CCF_MMC_DYNAMIC_EXTENSIONS clipboard format extends only non-namespace extensions. To dynamically add namespace extensions, the snap-in must use the 
<a href="https://msdn.microsoft.com/6057b8dd-d794-43a3-998b-689aafa28b9d">IConsoleNameSpace2::AddExtension</a> method. For more information, see 
<a href="https://msdn.microsoft.com/3dc9b2db-1fc0-495b-9acc-3366a24a18a7">Dynamic Namespace Extensions</a>.

Just before MMC must use an extensible feature (that is, just before creating and that displays a context menu, property sheet, toolbar, or taskpad), MMC calls <b>IDataObject::GetDataHere</b> on the data object for the selected item and asks for dynamic extensions to add through the CCF_MMC_DYNAMIC_EXTENSIONS clipboard format. Based on CLSIDs passed in the 
<b>SMMCDynamicExtensions</b> structure, MMC attempts to add the specified extensions to the extensible feature. If an extension is unavailable or unregistered, MMC skips that extension and continues to the next CLSID passed in the structure.




## -see-also




<a href="https://msdn.microsoft.com/48d55143-7873-4c66-a4c9-bde5663cb7f1">CCF_MMC_DYNAMIC_EXTENSIONS</a>



<a href="https://msdn.microsoft.com/6057b8dd-d794-43a3-998b-689aafa28b9d">IConsoleNameSpace2::AddExtension</a>



<a href="https://msdn.microsoft.com/e17574ea-a6a9-440e-97cf-7b87f13bf21e">SMMCObjectTypes</a>
 

 

