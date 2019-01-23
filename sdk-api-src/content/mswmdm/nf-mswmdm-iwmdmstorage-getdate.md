---
UID: NF:mswmdm.IWMDMStorage.GetDate
title: IWMDMStorage::GetDate
author: windows-sdk-content
description: The GetDate method retrieves the date when the storage was last modified.
old-location: wmdm\iwmdmstorage_getdate.htm
tech.root: WMDM
ms.assetid: 53693e2f-f6d2-42cc-9387-798f8dc10556
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDate, GetDate method [windows Media Device Manager], GetDate method [windows Media Device Manager],IWMDMStorage interface, IWMDMStorage interface [windows Media Device Manager],GetDate method, IWMDMStorage.GetDate, IWMDMStorage::GetDate, IWMDMStorageGetDate, mswmdm/IWMDMStorage::GetDate, wmdm.iwmdmstorage_getdate
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
 - IWMDMStorage.GetDate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMStorage::GetDate


## -description



The <b>GetDate</b> method retrieves the date when the storage was last modified.




## -parameters




### -param pDateTimeUTC [out]

Pointer to a <b>WMDMDATETIME</b> structure specifying the date on which the storage object (file or folder) was last modified.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -remarks



The time is specified in coordinated universal time.


#### Examples

The following C++ code gets the "last modified" value from a storage passed in.


```cpp

// Get the "Last Modified" date
WMDMDATETIME lastModified;
hr = pStorage->GetDate(&lastModified);
// TODO: Display the last modified month, day, and year.

```





## -see-also




<a href="https://msdn.microsoft.com/1ede7c68-0169-4375-9b45-b0995ad14e44">IWMDMStorage Interface</a>
 

 

