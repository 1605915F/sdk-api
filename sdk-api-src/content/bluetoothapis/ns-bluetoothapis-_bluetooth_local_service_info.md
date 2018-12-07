---
UID: NS:bluetoothapis._BLUETOOTH_LOCAL_SERVICE_INFO
title: "_BLUETOOTH_LOCAL_SERVICE_INFO"
author: windows-sdk-content
description: Contains local service information for a Bluetooth device.
old-location: bluetooth\bluetooth_local_service_info.htm
tech.root: Bluetooth
ms.assetid: d16fe6f1-4b76-4dbe-825e-e3995d2b4961
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: BLUETOOTH_LOCAL_SERVICE_INFO, BLUETOOTH_LOCAL_SERVICE_INFO structure [Bluetooth], BLUETOOTH_LOCAL_SERVICE_INFO_STRUCT, _BLUETOOTH_LOCAL_SERVICE_INFO, bluetooth.bluetooth_local_service_info, bluetoothapis/BLUETOOTH_LOCAL_SERVICE_INFO
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bluetoothapis.h
req.include-header: Bthsdpdef.h, BluetoothAPIs.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - BluetoothAPIs.h
api_name:
 - BLUETOOTH_LOCAL_SERVICE_INFO
product: Windows
targetos: Windows
req.typenames: BLUETOOTH_LOCAL_SERVICE_INFO_STRUCT
req.redist: 
---

# _BLUETOOTH_LOCAL_SERVICE_INFO structure


## -description


The <b>BLUETOOTH_LOCAL_SERVICE_INFO</b> structure contains local service information for a Bluetooth device. This structure is used by the <a href="https://msdn.microsoft.com/836c7804-6747-4a0b-b97c-c8c4e00374ca">BluetoothSetLocalServiceInfo</a> function.


## -struct-fields




### -field Enabled

If <b>TRUE</b>, specifies that the advertised services are enabled; otherwise the advertised services are disabled.


### -field btAddr

A <a href="https://msdn.microsoft.com/en-us/library/Aa362897(v=VS.85).aspx">BLUETOOTH_ADDRESS</a> structure that contains the address of a remote device. This address is used when advertising services to a device.


### -field szName

The service name. The maximum length of this string, including the null terminator, is <b>BLUETOOTH_MAX_SERVICE_NAME_SIZE</b> (256).


### -field szDeviceString

The local device name, if any, such as  COM4 or LPT1. The maximum length of this string, including the null terminator, is <b>BLUETOOTH_DEVICE_NAME_SIZE</b> (256).


## -remarks



In the event  the service is not associated with a specific device, <b>btAddr</b> should be set to <b>BTH_ADDR_NULL</b>.




## -see-also




<a href="https://msdn.microsoft.com/836c7804-6747-4a0b-b97c-c8c4e00374ca">BluetoothSetLocalServiceInfo</a>
 

 

