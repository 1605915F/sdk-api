---
UID: NS:winreg.value_entW
title: VALENTW (winreg.h)
author: windows-sdk-content
description: Contains information about a registry value. The RegQueryMultipleValues function uses this structure.
old-location: base\valent_str.htm
tech.root: SysInfo
ms.assetid: 7881eea8-e4e3-48cf-ba8f-b5c23910ae7d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PVALENTW, PVALENT, PVALENT structure pointer, VALENT, VALENT structure, VALENTA, VALENTW, _win32_valent_str, base.valent_str, winreg/PVALENT, winreg/VALENT, winreg/VALENTA, winreg/VALENTW"
ms.topic: struct
req.header: winreg.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: VALENTW (Unicode) and VALENTA (ANSI)
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
 - Winreg.h
api_name:
 - VALENT
 - VALENTA
 - VALENTW
product: Windows
targetos: Windows
req.typenames: VALENTW, *PVALENTW
req.redist: 
---

# VALENTW structure


## -description


Contains information about a registry value. The 
<a href="https://msdn.microsoft.com/e718534a-6e68-40f5-9cdd-170ce9b5e6e5">RegQueryMultipleValues</a> function uses this structure.


## -struct-fields




### -field ve_valuename

The name of the value to be retrieved. Be sure to set this member before calling 
<a href="https://msdn.microsoft.com/e718534a-6e68-40f5-9cdd-170ce9b5e6e5">RegQueryMultipleValues</a>.


### -field ve_valuelen

The size of the data pointed to by <b>ve_valueptr</b>, in bytes.


### -field ve_valueptr

A pointer to the data for the value entry. This is a pointer to the value's data returned in the <b>lpValueBuf</b> buffer filled in by 
<a href="https://msdn.microsoft.com/e718534a-6e68-40f5-9cdd-170ce9b5e6e5">RegQueryMultipleValues</a>.


### -field ve_type

The type of data pointed to by <b>ve_valueptr</b>. For a list of the possible types, see 
<a href="https://msdn.microsoft.com/5fd828d6-4d62-4823-a2f1-15782b5cd28c">Registry Value Types</a>.


## -see-also




<a href="https://msdn.microsoft.com/e718534a-6e68-40f5-9cdd-170ce9b5e6e5">RegQueryMultipleValues</a>
 

 

