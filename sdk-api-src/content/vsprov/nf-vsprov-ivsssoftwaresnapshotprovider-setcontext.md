---
UID: NF:vsprov.IVssSoftwareSnapshotProvider.SetContext
title: IVssSoftwareSnapshotProvider::SetContext
author: windows-sdk-content
description: Sets the context for subsequent shadow copy-related operations.
old-location: base\ivsssoftwaresnapshotprovider_setcontext.htm
tech.root: vss
ms.assetid: 5e2ddd7e-dcb8-4a13-8889-2d0e9dd102f2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVssSoftwareSnapshotProvider interface,SetContext method, IVssSoftwareSnapshotProvider.SetContext, IVssSoftwareSnapshotProvider::SetContext, SetContext, SetContext method, SetContext method,IVssSoftwareSnapshotProvider interface, base.ivsssoftwaresnapshotprovider_setcontext, vsprov/IVssSoftwareSnapshotProvider::SetContext
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: vsprov.h
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
req.lib: VssApi.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - VssApi.lib
 - VssApi.dll
api_name:
 - IVssSoftwareSnapshotProvider.SetContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVssSoftwareSnapshotProvider::SetContext


## -description


Sets the context for subsequent shadow copy-related operations.


## -parameters




### -param lContext [in]

The context to be set. The context must be one of the supported values of <a href="https://msdn.microsoft.com/2efe3066-4b91-4501-bacb-4211b222e0c3">_VSS_SNAPSHOT_CONTEXT</a> or a supported combination of <a href="https://msdn.microsoft.com/0326a81e-036c-4548-9e09-29054e51fadd">_VSS_VOLUME_SNAPSHOT_ATTRIBUTES</a> and  <b>_VSS_SNAPSHOT_CONTEXT</b> values.


## -returns



The following are the valid return codes for this method.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The context was set successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_ACCESSDENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have sufficient backup privileges or is not an administrator.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One of the parameter values is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The caller is out of memory or other system resources.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VSS_E_BAD_STATE</b></dt>
</dl>
</td>
<td width="60%">
The context is frozen and cannot be changed.

</td>
</tr>
</table>
 




## -remarks



The default context for VSS shadow copies is VSS_CTX_BACKUP.

<b>Windows XP:  </b>The only supported context is the default context, VSS_CTX_BACKUP. Therefore, calling 
     <b>SetContext</b> under Windows XP returns
     E_NOTIMPL.

For more information about how the context that is set by 
    <b>SetContext</b> affects 
    how a shadow copy is created and managed, see 
    <a href="https://msdn.microsoft.com/de5f1a5b-6e90-4abc-a232-aea93636772f">Implementation Details for 
    Creating Shadow Copies</a>.
   

For a complete discussion of the permitted shadow copy contexts, see 
    <a href="https://msdn.microsoft.com/2efe3066-4b91-4501-bacb-4211b222e0c3">_VSS_SNAPSHOT_CONTEXT</a> and 
    <a href="https://msdn.microsoft.com/0326a81e-036c-4548-9e09-29054e51fadd">_VSS_VOLUME_SNAPSHOT_ATTRIBUTES</a>.
   




## -see-also




<a href="https://msdn.microsoft.com/5c95f2fb-c132-489c-af48-2ffafad0b41f">IVssSoftwareSnapshotProvider</a>
 

 

