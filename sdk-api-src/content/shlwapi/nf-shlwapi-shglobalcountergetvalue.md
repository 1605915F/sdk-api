---
UID: NF:shlwapi.SHGlobalCounterGetValue
title: SHGlobalCounterGetValue function (shlwapi.h)
author: windows-sdk-content
description: Gets the current value of a global counter.
old-location: shell\SHGlobalCounterGetValue.htm
tech.root: shell
ms.assetid: cf158770-c9af-4488-9ed0-486e9a528a65
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SHGlobalCounterGetValue, SHGlobalCounterGetValue function [Windows Shell], _shell_SHGlobalCounterGetValue, shell.SHGlobalCounterGetValue, shlwapi/SHGlobalCounterGetValue
ms.topic: function
req.header: shlwapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
req.dll: Shlwapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Shlwapi.dll
api_name:
 - SHGlobalCounterGetValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SHGlobalCounterGetValue function


## -description


Gets the current value of a global counter.


## -parameters




### -param id [in]

Type: <b>const <a href="https://msdn.microsoft.com/e96f40fb-3a95-41d2-a45f-a8d91fb544d3">SHGLOBALCOUNTER</a></b>

The <a href="https://msdn.microsoft.com/e96f40fb-3a95-41d2-a45f-a8d91fb544d3">SHGLOBALCOUNTER</a> for which to retrieve the current value.


## -returns



Type: <b>long</b>

The current value of the counter.




## -see-also




<a href="https://msdn.microsoft.com/e96f40fb-3a95-41d2-a45f-a8d91fb544d3">SHGLOBALCOUNTER</a>



<a href="https://msdn.microsoft.com/67b45cb9-9d8d-48ef-a7bc-9cd8824bdf2b">SHGlobalCounterDecrement</a>



<a href="https://msdn.microsoft.com/088efa01-b070-4384-b17a-311aefb0737c">SHGlobalCounterIncrement</a>
 

 

