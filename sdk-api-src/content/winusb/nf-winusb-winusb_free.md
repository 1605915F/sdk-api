---
UID: NF:winusb.WinUsb_Free
title: WinUsb_Free function
author: windows-sdk-content
description: The WinUsb_Free function releases all of the resources that WinUsb_Initialize allocated. This is a synchronous operation.
old-location: buses\winusb_free.htm
tech.root: usbref
ms.assetid: 0f453364-fb2b-4b29-a96d-37c1d0d22608
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WinUsb_Free, WinUsb_Free function [Buses], buses.winusb_free, winusb/WinUsb_Free, winusbfunc_5364f078-34b5-4844-ab20-60e601f036b9.xml
ms.topic: function
req.header: winusb.h
req.include-header: Winusb.h
req.target-type: Universal
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
req.lib: Winusb.lib
req.dll: Winusb.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Winusb.dll
api_name:
 - WinUsb_Free
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WinUsb_Free function


## -description


The <b>WinUsb_Free</b> function releases all of the resources that <a href="https://msdn.microsoft.com/258cf508-036a-4ade-95b2-4b36d1149ffd">WinUsb_Initialize</a> allocated. This is a synchronous operation.


## -parameters




### -param InterfaceHandle [in]

An opaque handle to an interface in the selected configuration. That handle must be created by a previous call to  <a href="https://msdn.microsoft.com/258cf508-036a-4ade-95b2-4b36d1149ffd">WinUsb_Initialize</a> or <a href="https://msdn.microsoft.com/1afc7b2f-4fb6-4ab4-8415-aaee9cd6ee0c">WinUsb_GetAssociatedInterface</a>.


## -returns



<b>WinUsb_Free</b> returns <b>TRUE</b>.




## -see-also




<a href="https://msdn.microsoft.com/8234d0b4-2c73-45fa-a8bf-566c64cc2858">WinUSB</a>



<a href="https://docs.microsoft.com/en-us/windows/iot-core/learn-about-hardware/hardwarecompatlist">WinUSB Functions</a>



<a href="https://msdn.microsoft.com/258cf508-036a-4ade-95b2-4b36d1149ffd">WinUsb_Initialize</a>
 

 

