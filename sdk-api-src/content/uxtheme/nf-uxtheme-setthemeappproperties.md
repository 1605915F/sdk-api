---
UID: NF:uxtheme.SetThemeAppProperties
title: SetThemeAppProperties function
author: windows-sdk-content
description: Sets the flags that determine how visual styles are implemented in the calling application.
old-location: controls\SetThemeAppProperties.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\userex\functions\setthemeappproperties.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetThemeAppProperties, SetThemeAppProperties function [Windows Controls], controls.SetThemeAppProperties, controls.inet_SetThemeAppProperties, inet_SetThemeAppProperties, inet_SetThemeAppProperties_cpp, uxtheme/SetThemeAppProperties
ms.topic: function
req.header: uxtheme.h
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
req.lib: UxTheme.lib
req.dll: UxTheme.dll (version 1.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - UxTheme.dll
api_name:
 - SetThemeAppProperties
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetThemeAppProperties function


## -description


Sets the flags that determine how visual styles are implemented in the calling application.


## -parameters




### -param dwFlags

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

<b>DWORD</b> that specifies one or more of the following bit flags, which can be combined with a logical OR.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>STAP_ALLOW_NONCLIENT</dt>
</dl>
</td>
<td width="60%">
Specifies that the nonclient areas of application windows will have visual styles applied.

</td>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>STAP_ALLOW_CONTROLS</dt>
</dl>
</td>
<td width="60%">
Specifies that the common controls used in an application will have visual styles applied.

</td>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>STAP_ALLOW_WEBCONTENT</dt>
</dl>
</td>
<td width="60%">
Specifies that web content displayed in an application will have visual styles applied.

</td>
</tr>
</table>
 


## -returns



This function does not return a value.




## -remarks



After you set the flags, send a <a href="https://msdn.microsoft.com/en-us/library/ms632650(v=VS.85).aspx">WM_THEMECHANGED</a> message to your application's main window for the changes to take effect. 



#### Examples

This example combines flags and calls this function as shown.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>DWORD dwFlags = (STAP_ALLOW_NONCLIENT | 
        STAP_ALLOW_CONTROLS | STAP_ALLOW_WEBCONTENT);
SetThemeAppProperties(dwFlags);
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773369(v=VS.85).aspx">GetThemeAppProperties</a>
 

 

