---
UID: NF:dinputd.IDirectInputJoyConfig8.Release
title: IDirectInputJoyConfig8::Release (dinputd.h)
author: windows-sdk-content
description: The IDirectInputJoyConfig8::Release method decreases the reference count of the DirectInputJoyConfig object by 1. This method is part of the IUnknown interface inherited by DirectInputJoyConfig.
old-location: hid\idirectinputjoyconfig8_release.htm
tech.root: hid
ms.assetid: 60aff330-3646-4bc8-b7f4-b779a2e0796d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDirectInputJoyConfig8 interface [Human Input Devices],Release method, IDirectInputJoyConfig8.Release, IDirectInputJoyConfig8::Release, Release, Release method [Human Input Devices], Release method [Human Input Devices],IDirectInputJoyConfig8 interface, di_ref_510ae21c-eb2d-472d-aef2-944d17e31f78.xml, dinputd/IDirectInputJoyConfig8::Release, hid.idirectinputjoyconfig8_release
ms.topic: method
req.header: dinputd.h
req.include-header: Dinputd.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - COM
api_location:
 - Dinputd.h
api_name:
 - IDirectInputJoyConfig8.Release
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirectInputJoyConfig8::Release


## -description


The <b>IDirectInputJoyConfig8::Release </b>method decreases the reference count of the DirectInputJoyConfig object by 1. This method is part of the <b>IUnknown</b> interface inherited by DirectInputJoyConfig.


## -parameters






## -returns



Returns the new reference count of the object.




## -remarks



The DirectInputJoyConfig object deallocates itself when its reference count reaches 0. Use the <a href="https://msdn.microsoft.com/04e10558-367e-495c-aa1a-43344f803c8a">IDirectInputJoyConfig8::AddRef</a> method to increase the reference count of the object by 1.



