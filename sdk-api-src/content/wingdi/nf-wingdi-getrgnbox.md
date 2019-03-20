---
UID: NF:wingdi.GetRgnBox
title: GetRgnBox function (wingdi.h)
author: windows-sdk-content
description: The GetRgnBox function retrieves the bounding rectangle of the specified region.
old-location: gdi\getrgnbox.htm
tech.root: gdi
ms.assetid: 42d06f7f-1bf3-418f-a3b9-c009cf2de10b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetRgnBox, GetRgnBox function [Windows GDI], _win32_GetRgnBox, gdi.getrgnbox, wingdi/GetRgnBox
ms.topic: function
req.header: wingdi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Gdi32.lib
req.dll: Gdi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - gdi32.dll
 - Ext-MS-Win-GDI-rgn-l1-1-0.dll
 - Ext-MS-Win-RTCore-GDI-rgn-l1-1-0.dll
 - ext-ms-win-rtcore-gdi-rgn-l1-1-1.dll
 - GDI32Full.dll
api_name:
 - GetRgnBox
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetRgnBox function


## -description


The <b>GetRgnBox</b> function retrieves the bounding rectangle of the specified region.


## -parameters




### -param hrgn [in]

A handle to the region.


### -param lprc [out]

A pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that receives the bounding rectangle in logical units.


## -returns



The return value specifies the region's complexity. It can be one of the following values:

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>NULLREGION</td>
<td>Region is empty.</td>
</tr>
<tr>
<td>SIMPLEREGION</td>
<td>Region is a single rectangle.</td>
</tr>
<tr>
<td>COMPLEXREGION</td>
<td>Region is more than a single rectangle.</td>
</tr>
</table>
 

If the <i>hrgn</i> parameter does not identify a valid region, the return value is zero.




## -see-also




<a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>



<a href="https://msdn.microsoft.com/3a42fc7a-4c07-4540-99a7-520f99532f33">Region Functions</a>



<a href="https://msdn.microsoft.com/5d2e8624-4d1a-44f7-821e-a54f6f538214">Regions Overview</a>
 

 

