---
UID: NF:vds.IVdsVolumeMF3.QueryVolumeGuidPathnames
title: IVdsVolumeMF3::QueryVolumeGuidPathnames (vds.h)
author: windows-sdk-content
description: Returns a list of volume GUID paths for the current volume.
old-location: base\ivdsvolumemf3_queryvolumeguidpathnames.htm
tech.root: VDS
ms.assetid: 08311403-23a9-4191-9720-3cec805de825
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVdsVolumeMF3 interface,QueryVolumeGuidPathnames method, IVdsVolumeMF3.QueryVolumeGuidPathnames, IVdsVolumeMF3::QueryVolumeGuidPathnames, QueryVolumeGuidPathnames, QueryVolumeGuidPathnames method, QueryVolumeGuidPathnames method,IVdsVolumeMF3 interface, base.ivdsvolumemf3_queryvolumeguidpathnames, vds/IVdsVolumeMF3::QueryVolumeGuidPathnames
ms.topic: method
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - IVdsVolumeMF3.QueryVolumeGuidPathnames
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVdsVolumeMF3::QueryVolumeGuidPathnames


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns a list of volume GUID paths for the current volume.


## -parameters




### -param pwszPathArray [out]

<a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a>

### -param pulNumberOfPaths [out]

A pointer to a variable that receives the number of volume GUID paths returned in the buffer pointed to by the <i>pwszPathArray</i> parameter.


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
The method completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INTERNAL_ERROR</b></dt>
<dt>0x80042448L</dt>
</dl>
</td>
<td width="60%">
An internal error occurred. Check the event log for more details.

</td>
</tr>
</table>
 




## -remarks



A volume GUID path is a string of the form "\\?\Volume{GUID}\" where GUID is a GUID that identifies the volume.




## -see-also




<a href="https://msdn.microsoft.com/46b8ff26-c00b-45ef-ac30-0aa82786bf9b">IVdsVolumeMF3</a>
 

 

