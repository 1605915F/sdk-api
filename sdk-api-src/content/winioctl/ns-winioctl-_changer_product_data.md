---
UID: NS:winioctl._CHANGER_PRODUCT_DATA
title: "_CHANGER_PRODUCT_DATA"
author: windows-sdk-content
description: Represents product data for a changer device. It is used by the IOCTL_CHANGER_GET_PRODUCT_DATA control code.
old-location: base\changer_product_data_str.htm
tech.root: devio
ms.assetid: b6756994-2c6f-4797-8fad-823d63632372
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCHANGER_PRODUCT_DATA, CHANGER_PRODUCT_DATA, CHANGER_PRODUCT_DATA structure, PCHANGER_PRODUCT_DATA, PCHANGER_PRODUCT_DATA structure pointer, _CHANGER_PRODUCT_DATA, _win32_changer_product_data_str, base.changer_product_data_str, winioctl/CHANGER_PRODUCT_DATA, winioctl/PCHANGER_PRODUCT_DATA"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winioctl.h
req.include-header: Windows.h
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
 - WinIoCtl.h
api_name:
 - CHANGER_PRODUCT_DATA
product: Windows
targetos: Windows
req.typenames: CHANGER_PRODUCT_DATA, *PCHANGER_PRODUCT_DATA
req.redist: 
---

# _CHANGER_PRODUCT_DATA structure


## -description


Represents product data for a changer device. It is used by the 
<a href="https://msdn.microsoft.com/60744666-fb37-4263-8f4a-e7e043e6b71e">IOCTL_CHANGER_GET_PRODUCT_DATA</a> control code.


## -struct-fields




### -field VendorId

The device manufacturer's name. This is acquired directly from the device inquiry data.


### -field ProductId

The product identification, as defined by the vendor. This is acquired directly from the device inquiry data.


### -field Revision

The product revision, as defined by the vendor.


### -field SerialNumber

A unique value used to globally identify this device, as defined by the vendor.


### -field DeviceType

The device type of data transports, as defined by SCSI-2. This member must be <b>FILE_DEVICE_CHANGER</b>.


## -see-also




<a href="https://msdn.microsoft.com/60744666-fb37-4263-8f4a-e7e043e6b71e">IOCTL_CHANGER_GET_PRODUCT_DATA</a>
 

 

