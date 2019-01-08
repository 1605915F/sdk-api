---
UID: NF:tpmvscmgr.ITpmVirtualSmartCardManager.DestroyVirtualSmartCard
title: ITpmVirtualSmartCardManager::DestroyVirtualSmartCard
author: windows-sdk-content
description: Destroys the TPM virtual smart card that has the given instance ID.
old-location: security\itpmvirtualsmartcardmanager_destroyvirtualsmartcard.htm
tech.root: SecAuthN
ms.assetid: C8624CBF-FC39-4269-9405-8E7B5EE88F8D
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DestroyVirtualSmartCard, DestroyVirtualSmartCard method [Security], DestroyVirtualSmartCard method [Security],ITpmVirtualSmartCardManager interface, ITpmVirtualSmartCardManager interface [Security],DestroyVirtualSmartCard method, ITpmVirtualSmartCardManager.DestroyVirtualSmartCard, ITpmVirtualSmartCardManager::DestroyVirtualSmartCard, security.itpmvirtualsmartcardmanager_destroyvirtualsmartcard, tpmvscmgr/ITpmVirtualSmartCardManager::DestroyVirtualSmartCard
ms.topic: method
req.header: tpmvscmgr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tpmvscmgr.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Vscmgr.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Vscmgr.lib
 - Vscmgr.dll
api_name:
 - ITpmVirtualSmartCardManager.DestroyVirtualSmartCard
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITpmVirtualSmartCardManager::DestroyVirtualSmartCard


## -description


Destroys the TPM virtual smart card that has the given instance ID.


## -parameters




### -param pszInstanceId [in]

Instance identifier of the TPM virtual smart card that is returned from a successful <a href="https://msdn.microsoft.com/C80C4DE2-0C43-40A5-81E6-7036A0B8DEB7">CreateVirtualSmartCard</a> method call. 


### -param pStatusCallback [in, optional]

Pointer to a <a href="https://msdn.microsoft.com/6CB62E42-16FD-453F-9566-B4DFCDAC7368">ITpmVirtualSmartCardManagerStatusCallback</a> interface. The TPM virtual smart card manager uses this callback interface to communicate the progress and errors during creation of the virtual smart card. If the <i>pStatusCallback</i> parameter is <b>NULL</b>, no progress is reported to the client before the operation completes.


### -param pfNeedReboot [out]

Pointer to a Boolean value to receive whether the requested operation needs to reboot the client computer.


## -returns



If the method succeeds, it returns <b>S_OK</b>.

If the method fails, it returns a Win32 error code. 




## -see-also




<a href="https://msdn.microsoft.com/46CC703B-14A2-4588-BA13-837C76B70F07">ITpmVirtualSmartCardManager</a>
 

 

