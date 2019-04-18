---
UID: NF:setupapi.SetupDiSelectDevice
title: SetupDiSelectDevice function (setupapi.h)
author: windows-sdk-content
description: The SetupDiSelectDevice function is the default handler for the DIF_SELECTDEVICE request.
old-location: devinst\setupdiselectdevice.htm
tech.root: devinst
ms.assetid: c6a512ad-bcc6-4dc5-873e-33bdaab129e2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SetupDiSelectDevice, SetupDiSelectDevice function [Device and Driver Installation], devinst.setupdiselectdevice, di-rtns_0cbab99d-4106-4e25-81fc-68034d9f464d.xml, setupapi/SetupDiSelectDevice
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
req.dll: Setupapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Setupapi.dll
api_name:
 - SetupDiSelectDevice
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SetupDiSelectDevice function


## -description


The <b>SetupDiSelectDevice</b> function is the default handler for the <a href="https://msdn.microsoft.com/c1266182-b88f-406a-876c-e0f15050fdf3">DIF_SELECTDEVICE</a> request.


## -parameters




### -param DeviceInfoSet [in]

A handle to a <a href="https://msdn.microsoft.com/library/Ff541247(v=VS.85).aspx">device information set</a> that contains a device information element that represents the device for which to select a driver.


### -param DeviceInfoData [in, out]

A pointer to an <a href="https://msdn.microsoft.com/9ad0ef4f-4a67-4f16-8bb1-2242dad0d041">SP_DEVINFO_DATA</a> structure that specifies the device information element. This parameter is optional and can be <b>NULL</b>. If this parameter is specified, <b>SetupDiSelectDevice</b> selects the driver for the specified device and sets <i>DeviceInfoData.</i><b>ClassGuid</b> to the GUID of the <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a> for the selected driver. If this parameter is <b>NULL</b>, <b>SetupDiSelectDevice</b> sets the selected driver in the global class driver list for <i>DeviceInfoSet</i>.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved by a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



<b>SetupDiSelectDevice</b> handles the user interface that allows the user to select a driver for the specified device, or a device information set if a device is not specified. By setting the <b>Flags</b> field of the <a href="https://msdn.microsoft.com/1bd21150-f8f4-480d-a4b2-99fa4b4233b9">SP_DEVINSTALL_PARAMS</a> structure for the device, or the device information set if a device is not specified, the caller can specify special handling of the user interface, for example, to allow users to select a driver from an OEM installation disk. 

<div class="alert"><b>Note</b>  Only a class installer should call <b>SetupDiSelectDevice</b> and only in those situations where the class installer must perform driver selection operations after <b>SetupDiSelectDevice</b> completes the default driver selection operation. In such situations, the class installer must directly call <b>SetupDiSelectDevice</b> when the installer processes a DIF_SELECTDEVICE request. For more information about calling the default handler, see <a href="https://msdn.microsoft.com/library/Ff537868(v=VS.85).aspx">Calling Default DIF Code Handlers</a>.</div>
<div> </div>
<b>SetupDiSelectDevice</b> is primarily designed to select a driver for a device on a local computer before installing the device. Although <b>SetupDiSelectDevice</b> will not fail if the device information set is for a remote computer, the result is of limited use because the device information set cannot subsequently be used with DIF_<i>Xxx</i> installation requests or <b>SetupDi</b><i>Xxx</i> functions that do not support operations on a remote computer. In particular, the device information set cannot be used as input with a DIF_INSTALLDEVICE installation request to install a device on a remote computer.




## -see-also




<a href="https://msdn.microsoft.com/1bd21150-f8f4-480d-a4b2-99fa4b4233b9">SP_DEVINSTALL_PARAMS</a>



<a href="https://msdn.microsoft.com/2aa631c3-8d00-4309-a37c-efaa7eda3efa">SetupDiCallClassInstaller</a>
 

 

