---
UID: NN:syncregistration.IEnumSyncProviderInfos
title: IEnumSyncProviderInfos
author: windows-sdk-content
description: Enumerates ISyncProviderInfo objects that contain the information used to create an instance of a synchronization provider.
old-location: winsync\ienumsyncproviderinfos.htm
tech.root: winsync
ms.assetid: 58b0dcc2-861a-4138-872a-cbbe2bb2cc4d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumSyncProviderInfos, IEnumSyncProviderInfos interface [Windows Sync], IEnumSyncProviderInfos interface [Windows Sync],described, syncregistration/IEnumSyncProviderInfos, winsync.ienumsyncproviderinfos
ms.topic: interface
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
 - IEnumSyncProviderInfos
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumSyncProviderInfos interface


## -description


Enumerates <a href="https://msdn.microsoft.com/b7c49533-d289-44b0-9a9e-cfa47af3a087">ISyncProviderInfo</a> objects that contain the information used to create an instance of a synchronization provider.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumSyncProviderInfos</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IEnumSyncProviderInfos</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumSyncProviderInfos</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/de53dade-82f3-418c-a44c-58d4b7502729">Clone</a>
</td>
<td align="left" width="63%">
Clones the enumerator and returns a new enumerator that is in the same state as the current one.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b56cacfd-9cfe-4f5a-a945-dca299e43497">Next</a>
</td>
<td align="left" width="63%">
Returns the next <b>ISyncProviderInfo</b> object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c2a7374b-fd57-4f50-b740-941625377b64">Reset</a>
</td>
<td align="left" width="63%">
Resets the enumerator to the beginning of the <b>ISyncProviderInfo</b> set.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/da59a26a-8df3-4a19-b771-6fd11f69576e">Skip</a>
</td>
<td align="left" width="63%">
Skips the specified number of <b>ISyncProviderInfo</b> objects.

</td>
</tr>
</table> 


## -remarks



This interface is obtained from the  <a href="https://msdn.microsoft.com/36a2b498-237e-418a-b5b8-5f9bcdfbe734">ISyncProviderRegistration::EnumerateSyncProviders</a> method. The method will return an  <b>IEnumSyncProviderInfos</b> enumerator for all registered <b>ISyncProviderInfo</b> objects or for just the registered <b>ISyncProviderInfo</b> objects that match the particular filter criteria.




## -see-also




<a href="https://msdn.microsoft.com/8233671e-bf89-448d-8347-9b4f0ae7501f">Windows Sync Registration Reference</a>
 

 

