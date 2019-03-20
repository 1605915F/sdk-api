---
UID: NS:vmr9._VMR9MonitorInfo
title: VMR9MonitorInfo (vmr9.h)
author: windows-sdk-content
description: The VMR9MonitorInfo structure is used with the VMR-9 in the IVMRMonitorConfig9::GetAvailableMonitors method to set and retrieve information about monitors on the system.
old-location: dshow\vmr9monitorinfo.htm
tech.root: DirectShow
ms.assetid: cb7d5c27-8762-450e-ba47-2a46e3106472
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: VMR9MonitorInfo, VMR9MonitorInfo structure [DirectShow], VMR9MonitorInfoStructure, dshow.vmr9monitorinfo, vmr9/VMR9MonitorInfo
ms.topic: struct
req.header: vmr9.h
req.include-header: 
req.target-type: Windows
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
 - HeaderDef
api_location:
 - Vmr9.h
api_name:
 - VMR9MonitorInfo
product: Windows
targetos: Windows
req.typenames: VMR9MonitorInfo
req.redist: 
---

# VMR9MonitorInfo structure


## -description



The <code>VMR9MonitorInfo</code> structure is used with the VMR-9 in the <a href="https://msdn.microsoft.com/en-us/library/Dd390483(v=VS.85).aspx">IVMRMonitorConfig9::GetAvailableMonitors</a> method to set and retrieve information about monitors on the system.




## -struct-fields




### -field uDevID

Integer index that specifies the monitor device.


### -field rcMonitor

Specifies the monitor's rectangle.


### -field hMon

Handle to the monitor.


### -field dwFlags

Flags as defined for the <a href="https://msdn.microsoft.com/f296ce29-3fc8-41c9-a201-56e222aa2219">MONITORINFOEX</a> structure. Currently the only valid flag is <b>MONITORINFOF_PRIMARY</b>, which indicates the primary display monitor.
          


### -field szDevice

Null-terminated string containing the device name.


### -field szDescription

Null-terminated string containing a description of the device.


### -field liDriverVersion

Specifies the driver version.


### -field dwVendorId

Specifies the vendor.


### -field dwDeviceId

Specifies the device ID.


### -field dwSubSysId

Specifies the device subsystem.


### -field dwRevision

Specifies the revision number.


## -remarks



This structure is used to configure monitors on multi-monitor systems.




## -see-also




<a href="https://msdn.microsoft.com/378f6f43-5c05-4ae4-be24-956f9fc0cacf">DirectShow Structures</a>
 

 

