---
UID: NF:dcomp.IDCompositionDevice.Commit
title: IDCompositionDevice::Commit
author: windows-sdk-content
description: Commits all DirectComposition commands that are pending on this device.
old-location: directcomp\idcompositiondevice_commit.htm
tech.root: directcomp
ms.assetid: 49a6d33d-7454-44be-b8ca-602b247d4eab
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Commit, Commit method [DirectComposition], Commit method [DirectComposition],IDCompositionDevice interface, IDCompositionDevice interface [DirectComposition],Commit method, IDCompositionDevice.Commit, IDCompositionDevice::Commit, dcomp/IDCompositionDevice::Commit, directcomp.idcompositiondevice_commit
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dcomp.lib
req.dll: Dcomp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dcomp.dll
api_name:
 - IDCompositionDevice.Commit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice::Commit


## -description


Commits all DirectComposition commands that are pending on this device.


## -parameters






## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



Calls to DirectComposition methods are always batched and executed atomically as a single transaction. Calls take effect only when <b>IDCompositionDevice::Commit</b> is called, at which time all pending method calls for a device are executed at once. 

An application that uses multiple devices must call <b>Commit</b> for each device separately. However, because the composition engine processes the calls individually, the batch of commands might not take effect at the same time. 


#### Examples

For an example, see <a href="https://msdn.microsoft.com/86006C3C-67A8-4931-BE76-D0CA9DB19505">How to Build a Simple Visual Tree</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/081a14ed-c152-4e0a-b85b-1111d825ce53">IDCompositionDevice</a>
 

 

