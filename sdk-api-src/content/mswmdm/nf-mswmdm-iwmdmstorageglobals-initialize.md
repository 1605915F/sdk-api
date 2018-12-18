---
UID: NF:mswmdm.IWMDMStorageGlobals.Initialize
title: IWMDMStorageGlobals::Initialize
author: windows-sdk-content
description: The Initialize method formats the storage medium.
old-location: wmdm\iwmdmstorageglobals_initialize.htm
tech.root: WMDM
ms.assetid: 9f5092f0-1c72-412b-af93-08bc78c750bc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMDMStorageGlobals interface [windows Media Device Manager],Initialize method, IWMDMStorageGlobals.Initialize, IWMDMStorageGlobals::Initialize, IWMDMStorageGlobalsInitialize, Initialize, Initialize method [windows Media Device Manager], Initialize method [windows Media Device Manager],IWMDMStorageGlobals interface, mswmdm/IWMDMStorageGlobals::Initialize, wmdm.iwmdmstorageglobals_initialize
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
 - IWMDMStorageGlobals.Initialize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMStorageGlobals::Initialize


## -description



The <b>Initialize</b> method formats the storage medium.




## -parameters




### -param fuMode [in]

Mode used to initialize the medium. Specify exactly one of the following two modes. If both modes are specified, block mode is used.

<table>
<tr>
<th>Mode
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>WMDM_MODE_BLOCK</td>
<td>The operation is performed using block mode processing. The call will not return until the operation is finished.</td>
</tr>
<tr>
<td>WMDM_MODE_THREAD</td>
<td>The operation is performed using thread mode processing. The call returns immediately, and the operation is performed in a background thread.</td>
</tr>
</table>
 


### -param pProgress [in]

Pointer to an <b>IWMDMProgress</b> interface implemented by an application to track the progress of the formatting operation.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -remarks



If an application uses WMDM_MODE_THREAD and passes a non-null <i>pProgress</i> parameter, the application must ensure that the object to which <i>pProgress</i> belongs is not destroyed until the read operation completes, because Windows Media Device Manager will send progress notifications to this object. This object can be destroyed only after it receives an <a href="https://msdn.microsoft.com/0edddd8c-8144-40dc-801c-eb8c899be249">End</a> notification. Failure to do this will result in access violations.




## -see-also




<a href="https://msdn.microsoft.com/9af022a6-19b4-41b7-b951-0acad6aab4a2">IWMDMProgress Interface</a>



<a href="https://msdn.microsoft.com/fe164271-58f0-4b28-a200-6b15f8b42d36">IWMDMStorageGlobals Interface</a>
 

 

