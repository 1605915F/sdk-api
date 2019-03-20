---
UID: NF:bluetoothapis.BluetoothRegisterForAuthenticationEx
title: BluetoothRegisterForAuthenticationEx function (bluetoothapis.h)
author: windows-sdk-content
description: The BluetoothRegisterForAuthenticationEx function registers an application for a pin request, numeric comparison and callback function.
old-location: bluetooth\bluetoothregisterforauthenticationex.htm
tech.root: bluetooth
ms.assetid: c9838f27-3450-4d51-be58-ce515d06d5cb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BluetoothRegisterForAuthenticationEx, BluetoothRegisterForAuthenticationEx function [Bluetooth], bluetooth.bluetoothregisterforauthenticationex, bluetoothapis/BluetoothRegisterForAuthenticationEx
ms.topic: function
req.header: bluetoothapis.h
req.include-header: Bthsdpdef.h, BluetoothAPIs.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Bthprops.lib
req.dll: Bthprops.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Bthprops.dll
 - BluetoothAPIs.dll
 - Ext-MS-Win-Bluetooth-APIs-l1-1-0.dll
api_name:
 - BluetoothRegisterForAuthenticationEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# BluetoothRegisterForAuthenticationEx function


## -description


The <b>BluetoothRegisterForAuthenticationEx</b> function registers an application for a pin request,  numeric comparison and callback function.
<div class="alert"><b>Note</b>  This API is supported in Windows Vista SP2 and Windows 7.</div><div> </div>

## -parameters




### -param pbtdiIn [in, optional]

A pointer to a <a href="https://msdn.microsoft.com/41b14980-8217-4948-b084-1f44051d12f7">BLUETOOTH_DEVICE_INFO</a> structure that specifies the bluetooth address to be utilized for comparison.


### -param phRegHandleOut [out]

A pointer to a <b>HBLUETOOTH_AUTHENTICATION_REGISTRATION</b> handle associated with the registered application. Call <a href="https://msdn.microsoft.com/bfb1a18c-e5b1-4053-8652-5a76b196bebe">BluetoothUnregisterAuthentication</a> to close
the handle.


### -param pfnCallbackIn [in, optional]

The function that will be called when the authentication event          occurs. This function should match the prototype of <a href="https://msdn.microsoft.com/835a624f-c08d-402c-940b-4443e1b38d58">PFN_AUTHENTICATION_CALLBACK_EX</a>.


### -param pvParam [in, optional]

Optional parameter to be passed through to the callback function specified by <i>pfnCallbackIn</i>.          This parameter  can be anything the application is required to define.


## -returns



Returns ERROR_SUCCESS upon successful completion; returns the following error codes upon failure:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Out of memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Win32 Error</b></dt>
</dl>
</td>
<td width="60%">
The registration handle that was provided is invalid.

</td>
</tr>
</table>
 




## -remarks



The caller must provide a valid callback address and must unregister the callback once notification is no longer required.  The deregistration of an authenticated device can be accomplished by calling <a href="https://msdn.microsoft.com/bfb1a18c-e5b1-4053-8652-5a76b196bebe">BluetoothUnregisterAuthentication</a>.

In scenarios where an application registers for authentication more than once, only the first callback function registered via this function will be called in the application while authentication is in progress.




## -see-also




<a href="https://msdn.microsoft.com/f85dd076-9062-413f-863f-9d3baba322ad">BluetoothRegisterForAuthentication</a>



<a href="https://msdn.microsoft.com/bfb1a18c-e5b1-4053-8652-5a76b196bebe">BluetoothUnregisterAuthentication</a>
 

 

