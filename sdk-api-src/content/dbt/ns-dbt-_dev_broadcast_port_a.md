---
UID: NS:dbt._DEV_BROADCAST_PORT_A
title: "_DEV_BROADCAST_PORT_A"
author: windows-sdk-content
description: Contains information about a modem, serial, or parallel port.
old-location: base\dev_broadcast_port_str.htm
tech.root: devio
ms.assetid: b8789f1c-7d82-4637-bdb0-016a22b3bc8a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PDEV_BROADCAST_PORT_A, DEV_BROADCAST_PORT, DEV_BROADCAST_PORT structure, DEV_BROADCAST_PORT_A, PDEV_BROADCAST_PORT, PDEV_BROADCAST_PORT structure pointer, _DEV_BROADCAST_PORT_A, _win32_dev_broadcast_port_str, base.dev_broadcast_port_str, dbt/DEV_BROADCAST_PORT, dbt/PDEV_BROADCAST_PORT"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dbt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
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
 - Dbt.h
api_name:
 - DEV_BROADCAST_PORT
product: Windows
targetos: Windows
req.typenames: DEV_BROADCAST_PORT_A, *PDEV_BROADCAST_PORT_A
req.redist: 
---

# _DEV_BROADCAST_PORT_A structure


## -description


Contains information about a modem, serial, or parallel port.


## -struct-fields




### -field dbcp_size

The size of this structure, in bytes. This is the size of the members plus the actual length of the 
      <b>dbcp_name</b> string (the null character is accounted for by the declaration of 
      <b>dbcp_name</b> as a one-character array.)


### -field dbcp_devicetype

Set to <b>DBT_DEVTYP_PORT</b>.


### -field dbcp_reserved

Reserved; do not use.


### -field dbcp_name

A null-terminated string specifying the friendly name of the port or the device connected to the port. 
      Friendly names are intended to help the user quickly and accurately identify the device—for example, 
      "COM1" and "Standard 28800 bps Modem" are considered friendly names.


## -see-also




<a href="https://msdn.microsoft.com/4fc81fcb-b9fe-4016-b639-a43845af2c5f">DEV_BROADCAST_HDR</a>



<a href="https://msdn.microsoft.com/85ebbdca-94a0-4467-8d15-ee3a850e1cd9">Device Management Structures</a>



<a href="https://msdn.microsoft.com/b64a3983-ee75-4199-9778-1e5b7cec59e4">WM_DEVICECHANGE</a>
 

 

