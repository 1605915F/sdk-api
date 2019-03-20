---
UID: NF:tom.ITextFont2.GetAutospaceParens
title: ITextFont2::GetAutospaceParens (tom.h)
author: windows-sdk-content
description: Gets the East Asian &#0034;autospace parentheses&#0034; state.
old-location: controls\itextfont2_getautospaceparens.htm
tech.root: Controls
ms.assetid: fce60349-cded-4cab-b2e5-4fad02d11195
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAutospaceParens, GetAutospaceParens method [Windows Controls], GetAutospaceParens method [Windows Controls],ITextFont2 interface, ITextFont2 interface [Windows Controls],GetAutospaceParens method, ITextFont2.GetAutospaceParens, ITextFont2::GetAutospaceParens, controls.itextfont2_getautospaceparens, tom/ITextFont2::GetAutospaceParens
ms.topic: method
req.header: tom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextFont2.GetAutospaceParens
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextFont2::GetAutospaceParens


## -description


Gets the East Asian "autospace parentheses" state.


## -parameters




### -param pValue [out, retval]

Type: <b>long*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb787724(v=VS.85).aspx">tomBool</a> value that can be one of the following.

<table class="clsStd">
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td><b>tomTrue</b></td>
<td>Use East Asian autospace parentheses.</td>
</tr>
<tr>
<td><b>tomFalse</b></td>
<td>Do not use East Asian autospace parentheses.</td>
</tr>
<tr>
<td><b>tomUndefined</b></td>
<td>The AutospaceParens property is undefined.</td>
</tr>
</table>
 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the method succeeds, it returns <b>NOERROR</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/d2d43bfd-7cdf-458a-822d-e3965bfe2284">ITextFont2</a>



<a href="https://msdn.microsoft.com/9a9290e0-221e-454a-af9c-9d1bf5d37b5e">ITextFont2::SetAutospaceParens</a>
 

 

