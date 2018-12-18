---
UID: NF:mobsync.ISyncMgrSynchronize.EnumSyncMgrItems
title: ISyncMgrSynchronize::EnumSyncMgrItems
author: windows-sdk-content
description: Obtains the ISyncMgrEnumItems interface for the items that are handled by a registered application.
old-location: shell\syncmgr_isyncmgrsynchronize_enumsyncmgritems.htm
tech.root: shell
ms.assetid: 75f6ce68-237f-4228-adcf-f5ec929f49a7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnumSyncMgrItems, EnumSyncMgrItems method [Windows Shell], EnumSyncMgrItems method [Windows Shell],ISyncMgrSynchronize interface, ISyncMgrSynchronize interface [Windows Shell],EnumSyncMgrItems method, ISyncMgrSynchronize.EnumSyncMgrItems, ISyncMgrSynchronize::EnumSyncMgrItems, mobsync/ISyncMgrSynchronize::EnumSyncMgrItems, shell.syncmgr_isyncmgrsynchronize_enumsyncmgritems, syncmgr.isyncmgrsynchronize_enumsyncmgritems
ms.topic: method
req.header: mobsync.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
req.dll: Mobsync.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mobsync.dll
api_name:
 - ISyncMgrSynchronize.EnumSyncMgrItems
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISyncMgrSynchronize::EnumSyncMgrItems


## -description


Obtains the 
<a href="https://msdn.microsoft.com/d90e3a19-0ea8-4396-a6e7-dafe1dc9b2ec">ISyncMgrEnumItems</a> interface for the items that are handled by a registered application.


## -parameters




### -param ppSyncMgrEnumItems [out]

Type: <b><a href="https://msdn.microsoft.com/d90e3a19-0ea8-4396-a6e7-dafe1dc9b2ec">ISyncMgrEnumItems</a>**</b>

The address of the variable that receives a pointer to a valid 
<a href="https://msdn.microsoft.com/d90e3a19-0ea8-4396-a6e7-dafe1dc9b2ec">ISyncMgrEnumItems</a> interface.


## -returns



Type: <b>HRESULT</b>

This method supports the standard return values E_INVALIDARG, E_UNEXPECTED, and E_OUTOFMEMORY, and the following:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The enumeration interface is returned successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_SYNCMGR_MISSINGITEMS</b></dt>
</dl>
</td>
<td width="60%">
The enumeration interface object is returned successfully, but some items are missing. When this success code is returned, the synchronization manager does not remove any stored preferences for ItemIds that are not returned in the enumerator.

</td>
</tr>
</table>
 




## -remarks



The enumeration object that this method creates implements the 
<a href="https://msdn.microsoft.com/d90e3a19-0ea8-4396-a6e7-dafe1dc9b2ec">ISyncMgrEnumItems</a> interface, which is a standard enumeration interface that contains the <a href="https://msdn.microsoft.com/bb4ab08a-aa12-46f0-8c7d-82742b0b1538">Next</a>, <a href="https://msdn.microsoft.com/91265648-1294-423d-8e09-6d14eb0b6d9e">Reset</a>, <a href="https://msdn.microsoft.com/33bf4956-3d16-412c-9551-4ae3366ddd78">Clone</a>, and <a href="https://msdn.microsoft.com/f317306b-5317-4c5e-a5e6-fd2d8728bc52">Skip</a> methods.




## -see-also




<a href="https://msdn.microsoft.com/d90e3a19-0ea8-4396-a6e7-dafe1dc9b2ec">ISyncMgrEnumItems</a>



<a href="https://msdn.microsoft.com/bb821672-10b1-4fe6-a752-6cd1ccd1e49e">ISyncMgrSynchronize</a>
 

 

