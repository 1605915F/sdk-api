---
UID: NF:setupapi.SetupDiGetDeviceInterfaceDetailA
title: SetupDiGetDeviceInterfaceDetailA function (setupapi.h)
author: windows-sdk-content
description: The SetupDiGetDeviceInterfaceDetail function returns details about a device interface.
old-location: devinst\setupdigetdeviceinterfacedetail.htm
tech.root: devinst
ms.assetid: fb4963f1-0ed4-483d-9f39-dcbac493bf1d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SetupDiGetDeviceInterfaceDetail, SetupDiGetDeviceInterfaceDetail function [Device and Driver Installation], SetupDiGetDeviceInterfaceDetailA, SetupDiGetDeviceInterfaceDetailW, devinst.setupdigetdeviceinterfacedetail, di-rtns_5203864c-0bc7-4a59-bdb3-ddda0dbbbf98.xml, setupapi/SetupDiGetDeviceInterfaceDetail
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
req.lib: Setupapi.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Setupapi.lib
 - Setupapi.dll
api_name:
 - SetupDiGetDeviceInterfaceDetail
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SetupDiGetDeviceInterfaceDetailA function


## -description


The <b>SetupDiGetDeviceInterfaceDetail</b> function returns details about a device interface.


## -parameters




### -param DeviceInfoSet [in]

A pointer to the <a href="https://msdn.microsoft.com/library/Ff541247(v=VS.85).aspx">device information set</a> that contains the interface for which to retrieve details. This handle is typically returned by <a href="https://msdn.microsoft.com/31bb0fc8-0fb8-4122-b9e8-5ff8fbbd903b">SetupDiGetClassDevs</a>.


### -param DeviceInterfaceData [in]

A pointer to an <a href="https://msdn.microsoft.com/df142e95-aa1c-4d3e-90c6-bac86effbd5d">SP_DEVICE_INTERFACE_DATA</a> structure that specifies the interface in <i>DeviceInfoSet</i> for which to retrieve details. A pointer of this type is typically returned by <a href="https://msdn.microsoft.com/5095404d-2447-407e-99e2-dd3ef3c3b905">SetupDiEnumDeviceInterfaces</a>.


### -param DeviceInterfaceDetailData [out, optional]

A pointer to an <a href="https://msdn.microsoft.com/9dd44297-6e51-425d-a355-f2ea78757bf7">SP_DEVICE_INTERFACE_DETAIL_DATA</a> structure to receive information about the specified interface. This parameter is optional and can be <b>NULL</b>. This parameter must be <b>NULL</b> if <i>DeviceInterfaceDetailSize</i> is zero. If this parameter is specified, the caller must set <i>DeviceInterfaceDetailData</i><b>.cbSize</b> to <b>sizeof</b>(SP_DEVICE_INTERFACE_DETAIL_DATA) before calling this function. The <b>cbSize</b> member always contains the size of the fixed part of the data structure, not a size reflecting the variable-length string at the end.


### -param DeviceInterfaceDetailDataSize [in]

The size of the <i>DeviceInterfaceDetailData</i> buffer. The buffer must be at least (<b>offsetof</b>(SP_DEVICE_INTERFACE_DETAIL_DATA, <b>DevicePath</b>) + <b>sizeof</b>(TCHAR)) bytes, to contain the fixed part of the structure and a single <b>NULL</b> to terminate an empty MULTI_SZ string. 

This parameter must be zero if <i>DeviceInterfaceDetailData</i> is <b>NULL</b>.


### -param RequiredSize [out, optional]

A pointer to a variable of type DWORD that receives the required size of the <i>DeviceInterfaceDetailData</i> buffer. This size includes the size of the fixed part of the structure plus the number of bytes required for the variable-length device path string. This parameter is optional and can be <b>NULL</b>.


### -param DeviceInfoData [out, optional]

A pointer to a buffer that receives information about the device that supports the requested interface. The caller must set <i>DeviceInfoData</i><b>.cbSize</b> to <b>sizeof</b>(SP_DEVINFO_DATA). This parameter is optional and can be <b>NULL</b>.


## -returns



<b>SetupDiGetDeviceInterfaceDetail</b> returns <b>TRUE</b> if the function completed without error. If the function completed with an error, <b>FALSE</b> is returned and the error code for the failure can be retrieved by calling <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



Using this function to get details about an interface is typically a two-step process:

<ol>
<li>
Get the required buffer size. Call <b>SetupDiGetDeviceInterfaceDetail</b> with a <b>NULL</b><i>DeviceInterfaceDetailData</i> pointer, a <i>DeviceInterfaceDetailDataSize</i> of zero, and a valid <i>RequiredSize</i> variable. In response to such a call, this function returns the required buffer size at <i>RequiredSize</i> and fails with <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> returning ERROR_INSUFFICIENT_BUFFER.

</li>
<li>
Allocate an appropriately sized buffer and call the function again to get the interface details.

</li>
</ol>
The interface detail returned by this function consists of a device path that can be passed to Win32 functions such as <a href="https://msdn.microsoft.com/80a96083-4de9-4422-9705-b8ad2b6cbd1b">CreateFile</a>. Do not attempt to parse the device path symbolic name. The device path can be reused across system starts.

<b>SetupDiGetDeviceInterfaceDetail</b> can be used to get just the <i>DeviceInfoData</i>. If the interface exists but <i>DeviceInterfaceDetailData</i> is <b>NULL</b>, this function fails, <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> returns ERROR_INSUFFICIENT_BUFFER, and the <i>DeviceInfoData</i> structure is filled with information about the device that exposes the interface.




## -see-also




<a href="https://msdn.microsoft.com/5095404d-2447-407e-99e2-dd3ef3c3b905">SetupDiEnumDeviceInterfaces</a>



<a href="https://msdn.microsoft.com/31bb0fc8-0fb8-4122-b9e8-5ff8fbbd903b">SetupDiGetClassDevs</a>
 

 

