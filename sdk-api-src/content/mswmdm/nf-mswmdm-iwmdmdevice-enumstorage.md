---
UID: NF:mswmdm.IWMDMDevice.EnumStorage
title: IWMDMDevice::EnumStorage (mswmdm.h)
author: windows-sdk-content
description: The EnumStorage method retrieves an IWMDMEnumStorage interface to enumerate the storages on a device.
old-location: wmdm\iwmdmdevice_enumstorage.htm
tech.root: WMDM
ms.assetid: ffd3c51a-7ec2-4ce5-9260-2b08bfa88a99
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EnumStorage, EnumStorage method [windows Media Device Manager], EnumStorage method [windows Media Device Manager],IWMDMDevice interface, IWMDMDevice interface [windows Media Device Manager],EnumStorage method, IWMDMDevice.EnumStorage, IWMDMDevice::EnumStorage, IWMDMDeviceEnumStorage, mswmdm/IWMDMDevice::EnumStorage, wmdm.iwmdmdevice_enumstorage
ms.topic: method
req.header: mswmdm.h
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
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mssachlp.lib
 - mssachlp.dll
api_name:
 - IWMDMDevice.EnumStorage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMDevice::EnumStorage


## -description



The <b>EnumStorage</b> method retrieves an <a href="https://msdn.microsoft.com/6ea80ab2-718b-464e-a805-9910460931bb">IWMDMEnumStorage</a> interface to enumerate the storages on a device.



Syntax


## -parameters




### -param ppEnumStorage [out]

Pointer to a pointer to an <a href="https://msdn.microsoft.com/6ea80ab2-718b-464e-a805-9910460931bb">IWMDMEnumStorage</a> interface to enumerate the storages on a device. This points to the root storage on the device. The caller is responsible for calling <b>Release</b> on the retrieved interface.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/8b171b8a-00b7-4873-a4f7-1a0f29ad5cc0">Exploring a Device</a>



<a href="https://msdn.microsoft.com/44212da9-a38a-4ed5-86af-cf60b40bb54d">IWMDMDevice Interface</a>



<a href="https://msdn.microsoft.com/6ea80ab2-718b-464e-a805-9910460931bb">IWMDMEnumStorage Interface</a>
 

 

