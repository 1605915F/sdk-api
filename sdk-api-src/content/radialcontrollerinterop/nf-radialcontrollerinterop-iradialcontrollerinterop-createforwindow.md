---
UID: NF:radialcontrollerinterop.IRadialControllerInterop.CreateForWindow
title: IRadialControllerInterop::CreateForWindow (radialcontrollerinterop.h)
author: windows-sdk-content
description: Instantiates a RadialController object and binds it to the active application.
old-location: input_radial\iradialcontrollerinterop_createforwindow.htm
tech.root: Input_Radial
ms.assetid: fe419ce2-9767-42c4-aaa6-a9b9ea93ec3e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CreateForWindow, CreateForWindow method, CreateForWindow method,IRadialControllerInterop interface, IRadialControllerInterop interface,CreateForWindow method, IRadialControllerInterop.CreateForWindow, IRadialControllerInterop::CreateForWindow, Input_Radial.iradialcontrollerinterop_createforwindow, radialcontrollerinterop/IRadialControllerInterop::CreateForWindow
ms.topic: method
req.header: radialcontrollerinterop.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1607 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: RadialControllerInterop.idl
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
 - COM
api_location:
 - RadialControllerInterop.h
api_name:
 - IRadialControllerInterop.CreateForWindow
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRadialControllerInterop::CreateForWindow


## -description


Instantiates a <a href="https://msdn.microsoft.com/5cd9534d-bdd7-49fa-81c7-a5ddca4e851a">RadialController</a> object and binds it to the active application.


## -parameters




### -param hwnd [in]

Handle to the window of the active application.


### -param riid [in]

The GUID for the resource interface.

The REFIID, or GUID, of the interface to the resource can be obtained by using the __uuidof() macro. For example, __uuidof(IRadialController) will get the GUID of the interface to a buffer resource.


### -param ppv [out]

Address of a pointer to a <a href="https://msdn.microsoft.com/5cd9534d-bdd7-49fa-81c7-a5ddca4e851a">RadialController</a> object.


## -returns



If this function succeeds, it returns <b>S_OK</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<b>Developer and UX guidance</b>



<a href="https://msdn.microsoft.com/ed701930-fae7-4c42-9e6b-b1cb3fac861c">IRadialControllerInterop</a>



<b>Samples</b>



<a href="https://go.microsoft.com/fwlink/?linkid=832322">Surface Dial interactions</a>



<a href="https://go.microsoft.com/fwlink/?linkid=832713">Universal Windows Platform samples (C# and C++)</a>



<a href="https://aka.ms/radialcontrollerclassicsample">Windows classic desktop sample</a>
 

 

