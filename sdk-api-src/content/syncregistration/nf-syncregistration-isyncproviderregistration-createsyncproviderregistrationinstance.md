---
UID: NF:syncregistration.ISyncProviderRegistration.CreateSyncProviderRegistrationInstance
title: ISyncProviderRegistration::CreateSyncProviderRegistrationInstance
author: windows-sdk-content
description: Creates an in-memory instance of a synchronization provider.
old-location: winsync\isyncproviderregistration_createsyncproviderregistrationinstance.htm
tech.root: winsync
ms.assetid: 637cf465-5d43-42d3-b7b9-3bd674135038
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateSyncProviderRegistrationInstance, CreateSyncProviderRegistrationInstance method [Windows Sync], CreateSyncProviderRegistrationInstance method [Windows Sync],ISyncProviderRegistration interface, ISyncProviderRegistration interface [Windows Sync],CreateSyncProviderRegistrationInstance method, ISyncProviderRegistration.CreateSyncProviderRegistrationInstance, ISyncProviderRegistration::CreateSyncProviderRegistrationInstance, syncregistration/ISyncProviderRegistration::CreateSyncProviderRegistrationInstance, winsync.isyncproviderregistration_createsyncproviderregistrationinstance
ms.topic: method
req.header: syncregistration.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Syncregistration.h
api_name:
 - ISyncProviderRegistration.CreateSyncProviderRegistrationInstance
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISyncProviderRegistration::CreateSyncProviderRegistrationInstance


## -description


Creates an in-memory instance of a synchronization provider.


## -parameters




### -param pProviderConfiguration [in]

A <a href="https://msdn.microsoft.com/en-us/library/Dd317253(v=VS.85).aspx">SyncProviderConfiguration</a> structure that contains the synchronization provider registration information.


### -param ppProviderInfo [out]

Returns a pointer to an <a href="https://msdn.microsoft.com/fe50e34c-6499-4c1e-b891-7b4f797510f2">ISyncProviderInfo</a> interface that is used to obtain information about the synchronization provider and access the configuration property store in order to store the synchronization provider configuration.


## -returns



The possible return codes include, but are not limited to, the values shown in the following table.

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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
Invalid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>SYNC_E_REGISTRATION_ALREADYREGISTERED </b></dt>
</dl>
</td>
<td width="60%">
The same unique instance ID has already been registered for a synchronization provider.

</td>
</tr>
</table>
 




## -remarks



The synchronization provider is not registered on the system until the <b>ISyncProviderInfo::Commit</b> method is called. This method is inherited by <a href="https://msdn.microsoft.com/fe50e34c-6499-4c1e-b891-7b4f797510f2">ISyncProviderInfo</a> from <b>IPropertyStore</b>. For an example of this, see <a href="https://msdn.microsoft.com/0d496730-a4db-4898-aad9-1b5ca3b8ea51">Overview of Registering a Synchronization Provider</a>.




## -see-also




<a href="https://msdn.microsoft.com/e7cf0c05-9d07-4630-ae34-9a9dd81492b2">ISyncProviderRegistration Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd317253(v=VS.85).aspx">SyncProviderConfiguration Structure</a>
 

 

