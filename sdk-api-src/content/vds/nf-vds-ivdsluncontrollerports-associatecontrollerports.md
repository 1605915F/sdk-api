---
UID: NF:vds.IVdsLunControllerPorts.AssociateControllerPorts
title: IVdsLunControllerPorts::AssociateControllerPorts
author: windows-sdk-content
description: Sets the subsystem controller ports to active or inactive with respect to the LUN. This method replaces IVdsLun::AssociateControllers.
old-location: base\ivdsluncontrollerports_associatecontrollerports.htm
tech.root: VDS
ms.assetid: 3b889cb7-92e4-4c18-b9b9-768865895595
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AssociateControllerPorts, AssociateControllerPorts method [VDS], AssociateControllerPorts method [VDS],IVdsLunControllerPorts interface, IVdsLunControllerPorts interface [VDS],AssociateControllerPorts method, IVdsLunControllerPorts.AssociateControllerPorts, IVdsLunControllerPorts::AssociateControllerPorts, base.ivdsluncontrollerports_associatecontrollerports, vds/IVdsLunControllerPorts::AssociateControllerPorts, vdshwprv/IVdsLunControllerPorts::AssociateControllerPorts
ms.topic: method
req.header: vds.h
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
 - Vds.h
 - VdsHwPrv.h
api_name:
 - IVdsLunControllerPorts.AssociateControllerPorts
product: Windows
targetos: Windows
req.typenames: 
req.redist: VDS 1.1
---

# IVdsLunControllerPorts::AssociateControllerPorts


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Sets the subsystem controller ports to active or inactive with respect to the LUN. This method 
    replaces <a href="https://msdn.microsoft.com/2c3dc668-1745-49f4-9cd1-3bf0b322d0b2">IVdsLun::AssociateControllers</a>.


## -parameters




### -param pActiveControllerPortIdArray

A pointer to an array of controller port GUIDs. The provider sets these controller ports to active. This array 
      includes controller ports already set to active that are to remain active.


### -param lNumberOfActiveControllerPorts

The number of controller ports specified in the  <i>pActiveControllerPortIdArray</i> parameter.


### -param pInactiveControllerPortIdArray

A
      pointer to an array of controller port GUIDs. The provider sets these controller ports to inactive. This array 
      includes controller ports already set to inactive that are to remain inactive.


### -param lNumberOfInactiveControllerPorts

The number of controller ports specified in the  <i>pInactiveControllerPortIdArray</i> parameter.


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
<dt><b><b>VDS_E_PROVIDER_CACHE_CORRUPT</b></b></dt>
<dt>0x8004241FL</dt>
</dl>
</td>
<td width="60%">
The cache of the provider is corrupted. This indicates a software or communication problem inside a provider 
        that caches information about the attached devices. The caller can use the 
        <a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">IVdsHwProvider::Reenumerate</a> method 
        followed by the  <a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">IVdsHwProvider::Refresh</a> method to 
        restore the cache.
       

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_OBJECT_DELETED</b></b></dt>
<dt>0x8004240BL</dt>
</dl>
</td>
<td width="60%">
The LUN object is no longer present.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_OBJECT_STATUS_FAILED</b></b></dt>
<dt>0x80042431L</dt>
</dl>
</td>
<td width="60%">
The LUN is in a failed state and is unable to perform the requested operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_ANOTHER_CALL_IN_PROGRESS</b></b></dt>
<dt>0x80042404L</dt>
</dl>
</td>
<td width="60%">
Another operation is in progress. This operation cannot proceed until previous operations are complete.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_OBJECT_NOT_FOUND</b></b></dt>
<dt>0x80042405L</dt>
</dl>
</td>
<td width="60%">
One or more GUIDs of data type <b>VDS_OBJECT_ID</b> specified in 
        the <i>pActiveControllerPortIdArray</i> or 
        <i>pInactiveControllerPortIdArray</i> parameters do not refer to an existing object.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_NOT_SUPPORTED</b></b></dt>
<dt>0x80042400L</dt>
</dl>
</td>
<td width="60%">
This operation or combination of parameters is not supported by this provider.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/81e48874-8bc2-4b82-bcf8-ce87f99ca3ad">IVdsLunControllerPorts</a>
 

 

