---
UID: NS:setupapi._SP_DEVINFO_LIST_DETAIL_DATA_A
title: SP_DEVINFO_LIST_DETAIL_DATA_A (setupapi.h)
author: windows-sdk-content
description: An SP_DEVINFO_LIST_DETAIL_DATA structure contains information about a device information set, such as its associated setup class GUID (if it has an associated setup class).
old-location: devinst\sp_devinfo_list_detail_data.htm
tech.root: devinst
ms.assetid: 03e6c137-5a7f-443d-878f-5e5c6642dde9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PSP_DEVINFO_LIST_DETAIL_DATA_A, PSP_DEVINFO_LIST_DETAIL_DATA, PSP_DEVINFO_LIST_DETAIL_DATA structure pointer [Device and Driver Installation], SP_DEVINFO_LIST_DETAIL_DATA, SP_DEVINFO_LIST_DETAIL_DATA structure [Device and Driver Installation], SP_DEVINFO_LIST_DETAIL_DATA_A, devinst.sp_devinfo_list_detail_data, di-struct_8539bcfc-25ee-49f5-bc59-74efc6aae5bf.xml, setupapi/PSP_DEVINFO_LIST_DETAIL_DATA, setupapi/SP_DEVINFO_LIST_DETAIL_DATA"
ms.topic: struct
req.header: setupapi.h
req.include-header: Setupapi.h
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
 - setupapi.h
api_name:
 - SP_DEVINFO_LIST_DETAIL_DATA
product: Windows
targetos: Windows
req.typenames: SP_DEVINFO_LIST_DETAIL_DATA_A, *PSP_DEVINFO_LIST_DETAIL_DATA_A
req.redist: 
---

# SP_DEVINFO_LIST_DETAIL_DATA_A structure


## -description


An SP_DEVINFO_LIST_DETAIL_DATA structure contains information about a device information set, such as its associated setup class GUID (if it has an associated setup class).


## -struct-fields




### -field cbSize

The size, in bytes, of the SP_DEVINFO_LIST_DETAIL_DATA structure.


### -field ClassGuid

The setup class GUID that is associated with the device information set or GUID_NULL if there is no associated setup class.


### -field RemoteMachineHandle

If the device information set is for a remote computer, this member is a configuration manager machine handle for the remote computer. If the device information set is for the local computer, this member is <b>NULL</b>. 

This is typically the parameter that components use to access the remote computer. The <b>RemoteMachineName</b> contains a string, in case the component requires the name of the remote computer.


### -field RemoteMachineName

A NULL-terminated string that contains the name of the remote computer. If the device information set is for the local computer, this member is an empty string.


## -see-also




<a href="https://msdn.microsoft.com/3f624882-9ccc-4be1-92aa-8bba9f0022ea">SetupDiGetDeviceInfoListDetail</a>
 

 

