---
UID: NS:winioctl._DEVICE_DSM_OFFLOAD_READ_PARAMETERS
title: DEVICE_DSM_OFFLOAD_READ_PARAMETERS (winioctl.h)
author: windows-sdk-content
description: Contains parameters for the DeviceDsmAction_OffloadRead action for the IOCTL_STORAGE_MANAGE_DATA_SET_ATTRIBUTES control code.
old-location: base\device_dsm_offload_read_parameters.htm
tech.root: devio
ms.assetid: 20dd3e5b-90f4-45fc-8cc8-bf9e6d08a026
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDEVICE_DSM_OFFLOAD_READ_PARAMETERS, DEVICE_DSM_OFFLOAD_READ_PARAMETERS, DEVICE_DSM_OFFLOAD_READ_PARAMETERS structure, PDEVICE_DSM_OFFLOAD_READ_PARAMETERS, PDEVICE_DSM_OFFLOAD_READ_PARAMETERS structure pointer, base.device_dsm_offload_read_parameters, winioctl/DEVICE_DSM_OFFLOAD_READ_PARAMETERS, winioctl/PDEVICE_DSM_OFFLOAD_READ_PARAMETERS"
ms.topic: struct
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
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
 - WinIoCtl.h
api_name:
 - DEVICE_DSM_OFFLOAD_READ_PARAMETERS
product: Windows
targetos: Windows
req.typenames: DEVICE_DSM_OFFLOAD_READ_PARAMETERS, *PDEVICE_DSM_OFFLOAD_READ_PARAMETERS
req.redist: 
ms.custom: 19H1
---

# DEVICE_DSM_OFFLOAD_READ_PARAMETERS structure


## -description


Contains parameters for the <b>DeviceDsmAction_OffloadRead</b> action for the 
    <a href="https://msdn.microsoft.com/48e797ec-dad2-4a9e-9ccd-aaa65ece8da4">IOCTL_STORAGE_MANAGE_DATA_SET_ATTRIBUTES</a> 
    control code.


## -struct-fields




### -field Flags

Set to 0.


### -field TimeToLive

The time to live (TTL) for the token, in milliseconds.


### -field Reserved

Set to 0.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ee907416(v=VS.85).aspx">DEVICE_MANAGE_DATA_SET_ATTRIBUTES</a>



<a href="https://msdn.microsoft.com/85ebbdca-94a0-4467-8d15-ee3a850e1cd9">Device Management Structures</a>



<a href="https://msdn.microsoft.com/48e797ec-dad2-4a9e-9ccd-aaa65ece8da4">IOCTL_STORAGE_MANAGE_DATA_SET_ATTRIBUTES</a>



<a href="https://msdn.microsoft.com/93eaa8dd-b244-4fdd-abd4-c7cab46cb2a6">STORAGE_OFFLOAD_READ_OUTPUT</a>
 

 

