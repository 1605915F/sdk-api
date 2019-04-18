---
UID: NF:wdstptmgmt.IWdsTransportSetupManager.DeregisterContentProvider
title: IWdsTransportSetupManager::DeregisterContentProvider (wdstptmgmt.h)
author: windows-sdk-content
description: Enables an application run on a client computer to deregister a content provider. This makes the provider no longer available for use by the WDS transport server.
old-location: wds\iwdstransportsetupmanager_deregistercontentprovider.htm
tech.root: wds
ms.assetid: 56ec14a8-db20-41e5-8bd2-73b5a64e5542
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DeregisterContentProvider, DeregisterContentProvider method [Windows Deployment Services], DeregisterContentProvider method [Windows Deployment Services],IWdsTransportSetupManager interface, IWdsTransportSetupManager interface [Windows Deployment Services],DeregisterContentProvider method, IWdsTransportSetupManager.DeregisterContentProvider, IWdsTransportSetupManager::DeregisterContentProvider, wds.iwdstransportsetupmanager_deregistercontentprovider, wdstptmgmt/IWdsTransportSetupManager::DeregisterContentProvider
ms.topic: method
req.header: wdstptmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: Wdstptmgmt.tlb
req.lib: 
req.dll: Wdstptmgmt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wdstptmgmt.dll
api_name:
 - IWdsTransportSetupManager.DeregisterContentProvider
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWdsTransportSetupManager::DeregisterContentProvider


## -description


Enables an application run on a client computer   to deregister a content provider.  This makes the provider no longer available for use by the WDS transport server.


## -parameters




### -param bszName [in]

The name of the content provider to be deregistered.


## -returns



Standard HRESULT error values are used: S_OK for success; others for failure.




## -see-also




<a href="https://msdn.microsoft.com/b7b0dc9f-081e-472f-98f7-fe555a411ea3">IWdsTransportSetupManager</a>
 

 

