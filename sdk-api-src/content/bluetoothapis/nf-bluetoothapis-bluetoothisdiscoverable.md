---
UID: NF:bluetoothapis.BluetoothIsDiscoverable
title: BluetoothIsDiscoverable function
author: windows-sdk-content
description: The BluetoothIsDiscoverable function determines whether a Bluetooth radio or radios is discoverable.
old-location: bluetooth\bluetoothisdiscoverable.htm
tech.root: Bluetooth
ms.assetid: 33d34e36-dc17-4029-91bd-53ece5a93b4b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BluetoothIsDiscoverable, BluetoothIsDiscoverable function [Bluetooth], bluetooth.bluetoothisdiscoverable, bluetoothapis/BluetoothIsDiscoverable
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - BluetoothIsDiscoverable
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# BluetoothIsDiscoverable function


## -description


The <b>BluetoothIsDiscoverable</b> function determines whether a Bluetooth radio or radios is discoverable.


## -parameters




### -param hRadio

Valid local radio handle, or <b>NULL</b>. If <b>NULL</b>, discovery is determined for all local radios; if any radio is discoverable, the function call succeeds.


## -returns



Returns <b>TRUE</b> if at least one Bluetooth radio is discoverable. Returns <b>FALSE</b> if no Bluetooth radios are discoverable.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa362770(v=VS.85).aspx">BluetoothAuthenticateDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362772(v=VS.85).aspx">BluetoothAuthenticateMultipleDevices</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362776(v=VS.85).aspx">BluetoothEnableDiscovery</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362778(v=VS.85).aspx">BluetoothEnableIncomingConnections</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362799(v=VS.85).aspx">BluetoothIsConnectable</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362883(v=VS.85).aspx">BluetoothRegisterForAuthentication</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362893(v=VS.85).aspx">BluetoothSendAuthenticationResponse</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa362895(v=VS.85).aspx">BluetoothUnregisterAuthentication</a>
 

 

