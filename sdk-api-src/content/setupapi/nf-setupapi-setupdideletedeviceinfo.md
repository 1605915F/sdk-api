---
UID: NF:setupapi.SetupDiDeleteDeviceInfo
title: SetupDiDeleteDeviceInfo function (setupapi.h)
author: windows-sdk-content
description: The SetupDiDeleteDeviceInfo function deletes a device information element from a device information set. This function does not delete the actual device.
old-location: devinst\setupdideletedeviceinfo.htm
tech.root: devinst
ms.assetid: f510c42d-8488-4aad-a3a4-662fc8138d28
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SetupDiDeleteDeviceInfo, SetupDiDeleteDeviceInfo function [Device and Driver Installation], devinst.setupdideletedeviceinfo, di-rtns_9bc5c091-910a-4152-acdf-eae4d86cda05.xml, setupapi/SetupDiDeleteDeviceInfo
ms.topic: function
f1_keywords: ["setupapi/SetupDiDeleteDeviceInfo"]
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
 - SetupDiDeleteDeviceInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SetupDiDeleteDeviceInfo function


## -description


The <b>SetupDiDeleteDeviceInfo</b> function deletes a device information element from a device information set. This function does not delete the actual device.


## -parameters




### -param DeviceInfoSet [in]

A handle to the <a href="https://docs.microsoft.com/windows-hardware/drivers/install/device-information-sets">device information set</a> that contains the device information element to delete.


### -param DeviceInfoData [in]

A pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/setupapi/ns-setupapi-_sp_devinfo_data">SP_DEVINFO_DATA</a> structure that represents the device information element in <i>DeviceInfoSet </i>to delete.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved with a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



If the specified device information element is in use (for example, by a wizard page), the function fails. In this case, a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> returns ERROR_DEVINFO_DATA_LOCKED. This happens if a handle to a wizard page is retrieved with a call to <a href="https://docs.microsoft.com/windows-hardware/drivers/install/setupdigetwizardpage">SetupDiGetWizardPage</a> with this device information element specified and the DIWP_FLAG_USE_DEVINFO_DATA flag set. To delete this device information element, you must first close the wizard's HPROPSHEETPAGE handle.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdicreatedeviceinfoa">SetupDiCreateDeviceInfo</a>



<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdienumdeviceinfo">SetupDiEnumDeviceInfo</a>



<a href="https://docs.microsoft.com/windows-hardware/drivers/install/setupdigetwizardpage">SetupDiGetWizardPage</a>



<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdiopendeviceinfoa">SetupDiOpenDeviceInfo</a>
 

 

