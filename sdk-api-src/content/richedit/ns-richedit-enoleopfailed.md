---
UID: NS:richedit._enoleopfailed
title: ENOLEOPFAILED (richedit.h)
author: windows-sdk-content
description: Contains information about a failed operation.
old-location: controls\ENOLEOPFAILED.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\richeditcontrols\richeditcontrolreference\richeditstructures\enoleopfailed.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ENOLEOPFAILED, ENOLEOPFAILED structure [Windows Controls], _win32_ENOLEOPFAILED_str, _win32_ENOLEOPFAILED_str_cpp, controls.ENOLEOPFAILED, controls._win32_ENOLEOPFAILED_str, richedit/ENOLEOPFAILED
ms.topic: struct
req.header: richedit.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - Richedit.h
api_name:
 - ENOLEOPFAILED
product: Windows
targetos: Windows
req.typenames: ENOLEOPFAILED
req.redist: 
---

# ENOLEOPFAILED structure


## -description


Contains information about a failed operation.


## -struct-fields




### -field nmhdr

Type: <b><a href="https://msdn.microsoft.com/0c8b116b-82ad-495a-b19d-8c172e0b2608">NMHDR</a></b>


<a href="https://msdn.microsoft.com/0c8b116b-82ad-495a-b19d-8c172e0b2608">NMHDR</a> notification header. 


### -field iob

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a></b>

Object index.


### -field lOper

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a></b>

Operation that failed. This can be <b>OLEOP_DOVERB</b> to indicate that <a href="https://msdn.microsoft.com/fabd6a0a-7b0c-4c99-af22-8b117addd5f7">IOleObject::DoVerb</a> failed. 


### -field hr

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Error code returned by the object on the operation. 


## -see-also




<a href="https://msdn.microsoft.com/b674c36f-2454-473e-8e1c-368c0afd8c34">EN_OLEOPFAILED</a>



<a href="https://msdn.microsoft.com/fabd6a0a-7b0c-4c99-af22-8b117addd5f7">IOleObject::DoVerb</a>



<b>Other Resources</b>



<b>Reference</b>
 

 

