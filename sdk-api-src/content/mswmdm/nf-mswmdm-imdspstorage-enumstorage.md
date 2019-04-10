---
UID: NF:mswmdm.IMDSPStorage.EnumStorage
title: IMDSPStorage::EnumStorage (mswmdm.h)
author: windows-sdk-content
description: The EnumStorage method accesses the IMDSPEnumStorage interface to enumerate the individual storage media on a device.
old-location: wmdm\imdspstorage_enumstorage.htm
tech.root: WMDM
ms.assetid: 8b97d023-172f-4335-8d15-e5a4b67f24b8
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EnumStorage, EnumStorage method [windows Media Device Manager], EnumStorage method [windows Media Device Manager],IMDSPStorage interface, IMDSPStorage interface [windows Media Device Manager],EnumStorage method, IMDSPStorage.EnumStorage, IMDSPStorage::EnumStorage, IMDSPStorageEnumStorage, mswmdm/IMDSPStorage::EnumStorage, wmdm.imdspstorage_enumstorage
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
 - IMDSPStorage.EnumStorage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMDSPStorage::EnumStorage


## -description



The <b>EnumStorage</b> method accesses the <b>IMDSPEnumStorage</b> interface to enumerate the individual storage media on a device.




## -parameters




### -param ppEnumStorage [out]

Pointer to an <b>IMDSPEnumStorage</b> interface.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -remarks



The <b>IMDSPEnumStorage</b> interface returned will enumerate the nested storages in the storage that <b>IMDSPStorage</b> corresponds to. Thus all the storage objects in a hierarchical structure can be retrieved recursively.

This method must be implemented. It must not return WMDM_E_NOTSUPPORTED or E_NOTIMPL. For more information, see <a href="https://msdn.microsoft.com/582c9dd5-f8ab-48df-afb3-fba931ee0dea">Mandatory and Optional Interfaces</a>.




## -see-also




<a href="https://msdn.microsoft.com/bbf19979-8e09-476e-9401-443ab5e84866">IMDSPDevice::EnumStorage</a>



<a href="https://msdn.microsoft.com/fc2fed46-1f4d-4d53-a843-0f699b687a18">IMDSPEnumStorage Interface</a>



<a href="https://msdn.microsoft.com/f22b8a6d-7df8-4fea-9436-79b9ded25a40">IMDSPStorage Interface</a>
 

 

