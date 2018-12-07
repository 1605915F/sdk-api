---
UID: NF:icm.WcsSetCalibrationManagementState
title: WcsSetCalibrationManagementState function
author: windows-sdk-content
description: Enables or disables system management of the display calibration state.
old-location: wcs\wcssetcalibrationmanagementstate.htm
tech.root: WCS
ms.assetid: 64646448-c5a8-48a6-923e-fccf1cf63855
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: WcsSetCalibrationManagementState, WcsSetCalibrationManagementState function [Windows Color System], icm/WcsSetCalibrationManagementState, wcs.wcssetcalibrationmanagementstate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: icm.h
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
req.lib: Mscms.lib
req.dll: Mscms.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - mscms.dll
api_name:
 - WcsSetCalibrationManagementState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- WcsSetCalibrationManagementState
: 
---

# WcsSetCalibrationManagementState function


## -description


Enables or disables system management of the  display calibration state.


## -parameters




### -param bIsEnabled [in]

<b>TRUE</b> to enable system management of the display calibration state. <b>FALSE</b> to disable system management of the display calibration state.


## -returns



If this function succeeds, the return value is <b>TRUE</b>.

If this function fails, the return value is <b>FALSE</b>.




## -remarks



This function must be  called with elevated permissions for it to succeed.



