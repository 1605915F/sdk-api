---
UID: NF:winsxs.CreateAssemblyNameObject
title: CreateAssemblyNameObject function
author: windows-sdk-content
description: The CreateAssemblyNameObject function obtains an instance of the IAssemblyName interface.
old-location: setup\createassemblynameobject.htm
tech.root: SbsCs
ms.assetid: 1290a0b3-28f9-46fb-a98f-40b43bc0df1a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateAssemblyNameObject, CreateAssemblyNameObject function [Side-by-side Assemblies], setup.createassemblynameobject, winsxs/CreateAssemblyNameObject
ms.topic: function
req.header: winsxs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: Sxs.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - sxs.dll
api_name:
 - CreateAssemblyNameObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CreateAssemblyNameObject function


## -description


The <b>CreateAssemblyNameObject</b> function obtains an instance of the <a href="https://msdn.microsoft.com/304b8fb3-5d17-4af0-b070-450a40dc5cc9">IAssemblyName</a> interface.


## -parameters




### -param ppAssemblyNameObj

Pointer to a location that receives the <a href="https://msdn.microsoft.com/304b8fb3-5d17-4af0-b070-450a40dc5cc9">IAssemblyName</a> pointer.


### -param szAssemblyName

A pointer to a string value containing  the name of a side-by-side assembly. Depending on  <i>dwFlags</i>, this is a string representation of the fully-specified side-by-side assembly name or the Name portion of the assembly   name. The string value can be <b>NULL</b>.


### -param dwFlags

The value of this parameter can be a combination of <a href="https://msdn.microsoft.com/fdbb5eb0-0e45-483c-bcab-8b19a079800c">CREATE_ASM_NAME_OBJ_FLAGS</a> enumeration options or 0. If the value is <b>CANOF_PARSE_DISPLAY_NAME</b>, the <i>szAssemblyName</i> parameter contains a string representation of the fully-specified side-by-side assembly name and is parsed to the individual properties. If 0, <i>szAssemblyName</i> is the Name portion of the side-by-side assembly name.


### -param pvReserved

This parameter is reserved and must be <b>NULL</b>.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



