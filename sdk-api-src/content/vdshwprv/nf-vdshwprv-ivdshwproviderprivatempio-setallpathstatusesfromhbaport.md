---
UID: NF:vdshwprv.IVdsHwProviderPrivateMpio.SetAllPathStatusesFromHbaPort
title: IVdsHwProviderPrivateMpio::SetAllPathStatusesFromHbaPort
author: windows-sdk-content
description: Sets the statuses of paths originating from a particular HBA port to a specified status.
old-location: base\ivdshwproviderprivatempio_setallpathstatusesfromhbaport.htm
tech.root: vds
ms.assetid: 1fc25ca9-7cb4-438c-b9da-4bf93bd18a0c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsHwProviderPrivateMpio interface [VDS],SetAllPathStatusesFromHbaPort method, IVdsHwProviderPrivateMpio.SetAllPathStatusesFromHbaPort, IVdsHwProviderPrivateMpio::SetAllPathStatusesFromHbaPort, SetAllPathStatusesFromHbaPort, SetAllPathStatusesFromHbaPort method [VDS], SetAllPathStatusesFromHbaPort method [VDS],IVdsHwProviderPrivateMpio interface, base.ivdshwproviderprivatempio_setallpathstatusesfromhbaport, vdshwprv/IVdsHwProviderPrivateMpio::SetAllPathStatusesFromHbaPort
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: vdshwprv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
 - COM
api_location:
 - VdsHwPrv.h
api_name:
 - IVdsHwProviderPrivateMpio.SetAllPathStatusesFromHbaPort
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsHwProviderPrivateMpio::SetAllPathStatusesFromHbaPort


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Sets the statuses of paths originating from a particular HBA port to a specified status.


## -parameters




### -param hbaPortProp

The properties of the HBA port from which the paths to be set originate.  The only fields that need to be 
      provided are <b>wwnNode</b> and <b>wwnPort</b>.  The hardware provider 
      must ignore all other fields.


### -param status

The status (enumerated by the <a href="https://msdn.microsoft.com/f0682db1-9058-4514-abb2-c10b936d4f41">VDS_PATH_STATUS</a> enumeration) to set the paths.


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
<dt><b><b>S_OK</b></b></dt>
</dl>
</td>
<td width="60%">
The association name was successfully set.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_S_STATUSES_INCOMPLETELY_SET</b></b></dt>
<dt>0x00042702L</dt>
</dl>
</td>
<td width="60%">
At least one path's status was not successfully set due to a nonfatal error (for example, the status conflicts with 
        the current load balance policy).

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/fa60e832-1148-4ffb-bf70-bd7b27180cdd">IVdsHwProviderPrivateMpio</a>



<a href="https://msdn.microsoft.com/297ccb5c-3fa2-4bb0-bdd2-60d4685dc55c">VDS_HBAPORT_PROP</a>



<a href="https://msdn.microsoft.com/f0682db1-9058-4514-abb2-c10b936d4f41">VDS_PATH_STATUS</a>
 

 

