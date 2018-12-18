---
UID: NS:winuser.tagTPMPARAMS
title: TPMPARAMS
author: windows-sdk-content
description: Contains extended parameters for the TrackPopupMenuEx function.
old-location: menurc\tpmparams.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\menus\menureference\menustructures\tpmparams.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPTPMPARAMS, LPTPMPARAMS, LPTPMPARAMS structure pointer [Menus and Other Resources], TPMPARAMS, TPMPARAMS structure [Menus and Other Resources], _win32_TPMPARAMS_str, _win32_tpmparams_str_cpp, menurc.tpmparams, winui._win32_tpmparams_str, winuser/LPTPMPARAMS, winuser/TPMPARAMS"
ms.topic: struct
req.header: winuser.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Winuser.h
api_name:
 - TPMPARAMS
product: Windows
targetos: Windows
req.typenames: TPMPARAMS
req.redist: 
---

# TPMPARAMS structure


## -description


Contains extended parameters for the <a href="https://msdn.microsoft.com/86b8f21b-0dfe-462e-a34a-c80ee5c1d185">TrackPopupMenuEx</a> function.


## -struct-fields




### -field cbSize

Type: <b>UINT</b>

The size of structure, in bytes. 


### -field rcExclude

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a></b>

The rectangle to be excluded when positioning the window, in screen coordinates. 


## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/f00c0b76-fabb-4451-bd4e-30b465d4d235">Menus</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/86b8f21b-0dfe-462e-a34a-c80ee5c1d185">TrackPopupMenuEx</a>
 

 

