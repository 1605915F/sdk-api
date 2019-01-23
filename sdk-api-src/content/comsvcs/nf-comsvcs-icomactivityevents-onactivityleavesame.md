---
UID: NF:comsvcs.IComActivityEvents.OnActivityLeaveSame
title: IComActivityEvents::OnActivityLeaveSame
author: windows-sdk-content
description: Generated when an activity thread is left after being entered recursively.
old-location: cos\icomactivityevents_onactivityleavesame.htm
tech.root: cossdk
ms.assetid: 5a82fba1-a7d8-48d6-aa54-2f1a28e1b3d9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComActivityEvents interface [COM+],OnActivityLeaveSame method, IComActivityEvents.OnActivityLeaveSame, IComActivityEvents::OnActivityLeaveSame, OnActivityLeaveSame, OnActivityLeaveSame method [COM+], OnActivityLeaveSame method [COM+],IComActivityEvents interface, _dtc_IComActivityEvents_OnActivityLeaveSame, comsvcs/IComActivityEvents::OnActivityLeaveSame, cos.icomactivityevents_onactivityleavesame
ms.topic: method
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - ComSvcs.h
api_name:
 - IComActivityEvents.OnActivityLeaveSame
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComActivityEvents::OnActivityLeaveSame


## -description


Generated when an activity thread is left after being entered recursively.


## -parameters




### -param pInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms688276(v=VS.85).aspx">COMSVCSEVENTINFO</a> structure.


### -param guidCurrent [in]

The GUID associated with the caller.


### -param dwCallDepth [in]

The recursion depth.


## -returns



The user verifies the return values from this method.




## -see-also




<a href="https://msdn.microsoft.com/9b702bcd-d5a6-41fa-98ce-00a245dfe770">IComActivityEvents</a>
 

 

