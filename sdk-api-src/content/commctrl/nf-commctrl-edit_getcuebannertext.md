---
UID: NF:commctrl.Edit_GetCueBannerText
title: Edit_GetCueBannerText macro (commctrl.h)
author: windows-sdk-content
description: Gets the text that is displayed as a textual cue, or tip, in an edit control. You can use this macro or send the EM_GETCUEBANNER message explicitly.
old-location: controls\Edit_GetCueBannerText.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\editcontrols\editcontrolreference\editcontrolmacros\edit_getcuebannertext.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Edit_GetCueBannerText, Edit_GetCueBannerText macro [Windows Controls], _win32_Edit_GetCueBannerText, _win32_Edit_GetCueBannerText_cpp, commctrl/Edit_GetCueBannerText, controls.Edit_GetCueBannerText, controls._win32_Edit_GetCueBannerText
ms.topic: macro
req.header: commctrl.h
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
 - Commctrl.h
api_name:
 - Edit_GetCueBannerText
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Edit_GetCueBannerText macro


## -description


Gets the text that is displayed as a textual cue, or tip, in an edit control. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761572(v=VS.85).aspx">EM_GETCUEBANNER</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the edit control. 


### -param lpwText

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCWSTR</a></b>

A  pointer to a Unicode string that receives the text that is set as the cue banner. 


### -param cchText

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a></b>

A <b>LONG</b> that specifies the number of <b>WCHAR</b>s in the string referenced by <i>lpcwText</i>.


## -remarks



<div class="alert"><b>Note</b>  To use this macro, you must provide a manifest specifying Comclt32.dll version 6.0. For more information on manifests, see <a href="https://msdn.microsoft.com/en-us/library/Bb773175(v=VS.85).aspx">Enabling Visual Styles</a>.</div>
<div> </div>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb761572(v=VS.85).aspx">EM_GETCUEBANNER</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb775458(v=VS.85).aspx">Edit Controls</a>



<b>Reference</b>
 

 

