---
UID: NF:vds.IVdsDiskOnline.Offline
title: IVdsDiskOnline::Offline
author: windows-sdk-content
description: Takes the disk offline.Windows Vista:  This method is not supported until Windows Vista with Service Pack 1 (SP1). Use IVdsDisk2::SetSANMode instead.
old-location: base\ivdsdiskonline_offline.htm
tech.root: vds
ms.assetid: 3f27dd46-2fa1-4522-9d35-db78255c6d11
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsDiskOnline interface,Offline method, IVdsDiskOnline.Offline, IVdsDiskOnline::Offline, Offline, Offline method, Offline method,IVdsDiskOnline interface, base.ivdsdiskonline_offline, vds/IVdsDiskOnline::Offline
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista with SP1 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Uuid.lib
 - Uuid.dll
api_name:
 - IVdsDiskOnline.Offline
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsDiskOnline::Offline


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Takes the disk offline.<b>Windows Vista:  </b>This method is not supported until Windows Vista with Service Pack 1 (SP1). Use <a href="https://msdn.microsoft.com/17bdb6f4-7d85-4aa6-b89b-a752332cc224">IVdsDisk2::SetSANMode</a> instead.




## -parameters






## -returns



This method can return standard HRESULT values, such as E_INVALIDARG or E_OUTOFMEMORY, and <a href="https://msdn.microsoft.com/c9ddd3b7-f017-4880-976a-c879a40dc17b">VDS-specific return values</a>. It can also return converted <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>  using the <a href="https://msdn.microsoft.com/en-us/library/ms680746(v=VS.85).aspx">HRESULT_FROM_WIN32</a> macro. Errors can originate from VDS itself or from the underlying <a href="https://msdn.microsoft.com/b2f7628c-b567-40a9-9ad7-6c47077af5fb">VDS provider</a> that is being used. Possible return values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_FAILED_TO_OFFLINE_DISK</b></dt>
</dl>
</td>
<td width="60%">
The offline operation failed.

</td>
</tr>
</table>
 




## -remarks



If a dynamic disk is read/write and online, it can be made read-only and taken offline as follows:

<ol>
<li>For each volume on the disk, call the <a href="https://msdn.microsoft.com/1ef5a1e6-0e41-4077-9ae8-fe266f2623cc">IVdsVolumeMF::Dismount</a> method, setting the <i>bForce</i> and <i>bPermanent</i> parameters to <b>TRUE</b>.</li>
<li>Call the <b>Offline</b> method.</li>
<li>Set the read-only bit. (This is the <b>VDS_DF_READ_ONLY</b> flag in the <a href="https://msdn.microsoft.com/c7c09f95-9489-46fd-8b03-cabdee4521cf">VDS_DISK_PROP</a> structure.)</li>
</ol>
If a basic disk is read/write and online, it can be made read-only and taken offline the same way, but the order of the steps does not matter.




## -see-also




<a href="https://msdn.microsoft.com/f30ceaa0-ff4b-49fb-b140-b6725810cd06">IVdsDiskOnline</a>



<a href="https://msdn.microsoft.com/b3366bc7-18ca-4a90-b4e7-e6213a7cc002">IVdsDiskOnline::Online</a>
 

 

