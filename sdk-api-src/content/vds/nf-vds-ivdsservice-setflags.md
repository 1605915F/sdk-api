---
UID: NF:vds.IVdsService.SetFlags
title: IVdsService::SetFlags
author: windows-sdk-content
description: Sets service object flags.
old-location: base\ivdsservice_setflags.htm
tech.root: vds
ms.assetid: 9c82746e-fbf0-4754-b246-82a174410cef
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsService interface [VDS],SetFlags method, IVdsService.SetFlags, IVdsService::SetFlags, SetFlags, SetFlags method [VDS], SetFlags method [VDS],IVdsService interface, base.ivdsservice_setflags, vds/IVdsService::SetFlags
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - IVdsService.SetFlags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsService::SetFlags


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Sets service object flags.


## -parameters




### -param ulFlags [in]

The flags enumerated by <a href="https://msdn.microsoft.com/d14718bd-43a3-4775-a218-27c59f6995eb">VDS_SERVICE_FLAG</a>. Callers can set the <b>VDS_SVF_AUTO_MOUNT_OFF</b> flag.


## -returns



This method can return standard HRESULT values, such as E_INVALIDARG or E_OUTOFMEMORY, and <a href="https://msdn.microsoft.com/c9ddd3b7-f017-4880-976a-c879a40dc17b">VDS-specific return values</a>. It can also return converted <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>  using the <a href="https://msdn.microsoft.com/en-us/library/ms680746(v=VS.85).aspx">HRESULT_FROM_WIN32</a> macro. Errors can originate from VDS itself or from the underlying <a href="https://msdn.microsoft.com/b2f7628c-b567-40a9-9ad7-6c47077af5fb">VDS provider</a> that is being used. Possible return values include the following.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The flags were set successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INITIALIZED_FAILED</b></dt>
<dt>0x80042401L</dt>
</dl>
</td>
<td width="60%">
VDS failed to initialize. If an application calls this method before the service finishes initializing, the method is blocked until the initialization completes. If the initialization fails, this error is returned.

</td>
</tr>
</table>
 




## -remarks



Beginning with Windows 8 and Windows Server 2012, the <b>VDS_SVF_AUTO_MOUNT_OFF</b> is deprecated. Instead, use the <a href="https://msdn.microsoft.com/2da99388-8ee6-4e6b-98dc-52f12290c4dc">VDS_SAN_POLICY</a> enumeration to control default disk mounting behavior.




## -see-also




<a href="https://msdn.microsoft.com/6b081cc8-fe06-427f-b06d-831a1f1fef52">IVdsService</a>



<a href="https://msdn.microsoft.com/d14718bd-43a3-4775-a218-27c59f6995eb">VDS_SERVICE_FLAG</a>
 

 

