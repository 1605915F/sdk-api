---
UID: NF:cscobj.IEnumOfflineFilesItems.Clone
title: IEnumOfflineFilesItems::Clone (cscobj.h)
author: windows-sdk-content
description: Creates a new instance of the enumerator with the same enumeration state as the current one.
old-location: of\ienumofflinefilesitems_clone.htm
tech.root: offlinefiles
ms.assetid: cef0adaf-d342-4eab-b455-2b51b7d70066
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Clone, Clone method [Offline Files], Clone method [Offline Files],IEnumOfflineFilesItems interface, IEnumOfflineFilesItems interface [Offline Files],Clone method, IEnumOfflineFilesItems.Clone, IEnumOfflineFilesItems::Clone, cscobj/IEnumOfflineFilesItems::Clone, of.ienumofflinefilesitems_clone
ms.topic: method
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: CscSvc.dll; CscObj.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CscSvc.dll
 - CscObj.dll
api_name:
 - IEnumOfflineFilesItems.Clone
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumOfflineFilesItems::Clone


## -description


Creates a new instance of the enumerator with the same enumeration state as the current one.


## -parameters




### -param ppenum [out]

Address of an <a href="https://msdn.microsoft.com/9bb1fa14-74d2-4c6f-b8ba-47c6e78d7a4f">IEnumOfflineFilesItems</a> pointer variable that receives the interface pointer of the new enumeration object.


## -returns



Returns <b>S_OK</b> if the enumerator is created successfully, or an error value otherwise.




## -see-also




<a href="https://msdn.microsoft.com/9bb1fa14-74d2-4c6f-b8ba-47c6e78d7a4f">IEnumOfflineFilesItems</a>
 

 

