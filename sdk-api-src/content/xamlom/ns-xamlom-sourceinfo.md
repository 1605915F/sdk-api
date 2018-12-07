---
UID: NS:xamlom.SourceInfo
title: SourceInfo
author: windows-sdk-content
description: Represents information about an object’s XAML source document.
old-location: xaml_diagnostics\sourceinfo.htm
tech.root: xaml_diagnostics
ms.assetid: 09B08C62-EF16-4A35-BFE9-B2D1CAE9F285
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PSourceInfo, PSourceInfo structure pointer, SourceInfo, SourceInfo structure, xaml_diagnostics.sourceinfo, xamlom/PSourceInfo, xamlom/SourceInfo
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: xamlom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XamlOM.idl
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
 - xamlom.h
api_name:
 - SourceInfo
product: Windows
targetos: Windows
req.typenames: SourceInfo
req.redist: 
---

# SourceInfo structure


## -description


Represents information about an object’s XAML source document.


## -struct-fields




### -field FileName

The name of the source document file where the element is declared.


### -field LineNumber

The line number in the source document where the element is declared.


### -field ColumnNumber

The position on the line in the source document where the element is declared.


### -field CharPosition

The character position in the source document.


### -field Hash

The hash of the source document.

