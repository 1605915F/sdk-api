---
UID: NF:oleacc.IAccPropServices.SetHwndProp
title: IAccPropServices::SetHwndProp
author: windows-sdk-content
description: This method wraps SetPropValue, providing a convenient entry point for callers who are annotating HWND-based accessible elements. If the new value is a string, you can use IAccPropServices::SetHwndPropStr instead.
old-location: winauto\iaccpropservices_iaccpropservices__sethwndprop.htm
tech.root: WinAuto
ms.assetid: 00387897-5385-467d-9da4-4d71fce742b6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAccPropServices interface [Windows Accessibility],SetHwndProp method, IAccPropServices.SetHwndProp, IAccPropServices::SetHwndProp, SetHwndProp, SetHwndProp method [Windows Accessibility], SetHwndProp method [Windows Accessibility],IAccPropServices interface, _msaa_IAccPropServices_SetHwndProp, msaa.iaccpropservices_iaccpropservices__sethwndprop, oleacc/IAccPropServices::SetHwndProp, winauto.iaccpropservices_iaccpropservices__sethwndprop
ms.topic: method
req.header: oleacc.h
req.include-header: OleAcc.h Include Initguid.h first.
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
req.dll: Oleacc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Oleacc.dll
api_name:
 - IAccPropServices.SetHwndProp
product: Windows
targetos: Windows
req.typenames: 
req.redist: Active Accessibility 2.0 RDK on Windows NT 4.0 with SP6 and later and Windows 98
---

# IAccPropServices::SetHwndProp


## -description


This method wraps <a href="https://msdn.microsoft.com/c86acb70-fa77-4f95-8a99-e60872cdaa7e">SetPropValue</a>, providing a convenient entry point for callers who are annotating <b>HWND</b>-based accessible elements. If the new value is a string, you can use <a href="https://msdn.microsoft.com/68f09a23-56b2-4fae-98a2-616b17fb4e1f">IAccPropServices::SetHwndPropStr</a> instead.


## -parameters




### -param hwnd [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Identifies the accessible element that is to be annotated. This replaces the identity string.


### -param idObject [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

Identifies the accessible element that is to be annotated. This replaces the identity string.


### -param idChild [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

Identifies the accessible element that is to be annotated. This replaces the identity string.


### -param idProp [in]

Type: <b>MSAAPROPID</b>

Specifies which property of that element is to be annotated.


### -param var [in]

Type: <b>VARIANT</b>

Specifies a new value for that property.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If successful, returns S_OK.

Returns E_INVALIDARG if the <i>idProp</i> property is not supported.

May return other error codes under exceptional error conditions such as low memory.




## -remarks



By using this method, the caller does not have to obtain an identity string; it can specify the <i>hwnd</i>, <i>idObject</i>, and <i>idChild</i> parameters directly.




## -see-also




<a href="https://msdn.microsoft.com/7fd3f595-4897-481f-972e-04cf1a4c6046">ClearHwndProps</a>



<a href="https://msdn.microsoft.com/0474dacf-7aa1-4d12-bac2-1091676a1ced">IAccPropServices</a>



<a href="https://msdn.microsoft.com/05dbdf97-9b1a-439f-b3a1-b517733ec0a8">SetHwndPropServer</a>



<a href="https://msdn.microsoft.com/68f09a23-56b2-4fae-98a2-616b17fb4e1f">SetHwndPropStr</a>



<a href="https://msdn.microsoft.com/c86acb70-fa77-4f95-8a99-e60872cdaa7e">SetPropValue</a>
 

 

