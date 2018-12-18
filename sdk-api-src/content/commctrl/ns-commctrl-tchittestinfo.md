---
UID: NS:commctrl.tagTCHITTESTINFO
title: TCHITTESTINFO
author: windows-sdk-content
description: Contains information about a hit test. This structure supersedes the TC_HITTESTINFO structure.
old-location: controls\TCHITTESTINFO.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\tab\structures\tchittestinfo.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPTCHITTESTINFO, LPTCHITTESTINFO, LPTCHITTESTINFO structure pointer [Windows Controls], TCHITTESTINFO, TCHITTESTINFO structure [Windows Controls], TCHT_NOWHERE, TCHT_ONITEM, TCHT_ONITEMICON, TCHT_ONITEMLABEL, _win32_TCHITTESTINFO, _win32_TCHITTESTINFO_cpp, commctrl/LPTCHITTESTINFO, commctrl/TCHITTESTINFO, controls.TCHITTESTINFO, controls._win32_TCHITTESTINFO"
ms.topic: struct
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
 - TCHITTESTINFO
product: Windows
targetos: Windows
req.typenames: TCHITTESTINFO, *LPTCHITTESTINFO
req.redist: 
---

# TCHITTESTINFO structure


## -description


Contains information about a hit test. This structure supersedes the
		<b>TC_HITTESTINFO</b> structure. 


## -struct-fields




### -field pt

Type: <b><a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a></b>

Position to hit test, in client coordinates. 


### -field flags

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Variable that receives the results of a hit test. The tab control sets this member to one of the following values: 

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="TCHT_NOWHERE"></a><a id="tcht_nowhere"></a><dl>
<dt><b>TCHT_NOWHERE</b></dt>
</dl>
</td>
<td width="60%">
The position is not over a tab.

</td>
</tr>
<tr>
<td width="40%"><a id="TCHT_ONITEM"></a><a id="tcht_onitem"></a><dl>
<dt><b>TCHT_ONITEM</b></dt>
</dl>
</td>
<td width="60%">
The position is over a tab but not over its icon or its text. For owner-drawn tab controls, this value is specified if the position is anywhere over a tab.

</td>
</tr>
<tr>
<td width="40%"><a id="TCHT_ONITEMICON"></a><a id="tcht_onitemicon"></a><dl>
<dt><b>TCHT_ONITEMICON</b></dt>
</dl>
</td>
<td width="60%">
The position is over a tab's icon.

</td>
</tr>
<tr>
<td width="40%"><a id="TCHT_ONITEMLABEL"></a><a id="tcht_onitemlabel"></a><dl>
<dt><b>TCHT_ONITEMLABEL</b></dt>
</dl>
</td>
<td width="60%">
The position is over a tab's text. 

</td>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
</dl>
</td>
<td width="60%">
TCHT_ONITEM is a bitwise-OR operation on TCHT_ONITEMICON and TCHT_ONITEMLABEL.

</td>
</tr>
</table>
 


## -see-also




<a href="https://msdn.microsoft.com/0334f616-8d39-4460-a7f8-692a9ffab012">TCM_HITTEST</a>
 

 

