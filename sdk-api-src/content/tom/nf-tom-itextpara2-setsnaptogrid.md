---
UID: NF:tom.ITextPara2.SetSnapToGrid
title: ITextPara2::SetSnapToGrid
author: windows-sdk-content
description: Sets whether paragraph lines snap to a vertical grid that could be defined for the whole document.
old-location: controls\itextpara2_setsnaptogrid.htm
tech.root: controls
ms.assetid: 93116780-03e2-406b-8923-b9f02f53892d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextPara2 interface [Windows Controls],SetSnapToGrid method, ITextPara2.SetSnapToGrid, ITextPara2::SetSnapToGrid, SetSnapToGrid, SetSnapToGrid method [Windows Controls], SetSnapToGrid method [Windows Controls],ITextPara2 interface, controls.itextpara2_setsnaptogrid, tom/ITextPara2::SetSnapToGrid
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
 - ITextPara2.SetSnapToGrid
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextPara2::SetSnapToGrid


## -description


Sets whether paragraph lines snap to a vertical grid that could be defined for the whole document.


## -parameters




### -param Value [in]

Type: <b>long</b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb787724(v=VS.85).aspx">tomBool</a> value that can be one of the following.

<table class="clsStd">
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td><b>tomTrue</b></td>
<td>Paragraph lines snap to a vertical grid.</td>
</tr>
<tr>
<td><b>tomFalse</b></td>
<td>Paragraph lines do not snap to a grid.</td>
</tr>
<tr>
<td><b>tomToggle</b></td>
<td>Toggle the SnapToGrid property.</td>
</tr>
<tr>
<td><b>tomUndefined</b></td>
<td>The SnapToGrid property is undefined.</td>
</tr>
</table>
 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the method succeeds, it returns <b>NOERROR</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/31a0849f-c651-4178-b1ff-a4333bcde5d9">ITextPara2</a>



<a href="https://msdn.microsoft.com/ee5fd1d8-cd2d-4674-bb0f-6021a3115aac">ITextPara2::GetSnapToGrid</a>
 

 

