---
UID: NF:mswmdm.IWMDeviceManager.GetDeviceCount
title: IWMDeviceManager::GetDeviceCount (mswmdm.h)
author: windows-sdk-content
description: The GetDeviceCount method retrieves the number of portable devices that are currently connected to the computer.
old-location: wmdm\iwmdevicemanager_getdevicecount.htm
tech.root: WMDM
ms.assetid: efa8ccf6-c796-4ed7-8fe0-2e6570292aaa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDeviceCount, GetDeviceCount method [windows Media Device Manager], GetDeviceCount method [windows Media Device Manager],IWMDeviceManager interface, IWMDeviceManager interface [windows Media Device Manager],GetDeviceCount method, IWMDeviceManager.GetDeviceCount, IWMDeviceManager::GetDeviceCount, IWMDeviceManagerGetDeviceCount, mswmdm/IWMDeviceManager::GetDeviceCount, wmdm.iwmdevicemanager_getdevicecount
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
 - IWMDeviceManager.GetDeviceCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDeviceManager::GetDeviceCount


## -description



The <b>GetDeviceCount</b> method retrieves the number of portable devices that are currently connected to the computer.




## -parameters




### -param pdwCount [out]

Pointer to a <b>DWORD</b> specifying the count of known devices.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/c5935681-b530-4446-a026-7ddc74084d23">Enumerating Devices</a>



<a href="https://msdn.microsoft.com/cac68821-42fc-4833-bf2e-eec1768869e6">IWMDeviceManager Interface</a>
 

 

