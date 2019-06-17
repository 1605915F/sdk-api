---
UID: NF:cscobj.IOfflineFilesDirtyInfo.RemoteDirtyByteCount
title: IOfflineFilesDirtyInfo::RemoteDirtyByteCount (cscobj.h)
author: windows-sdk-content
description: This method is reserved for future use.
old-location: of\iofflinefilesdirtyinfo_remotedirtybytecount.htm
tech.root: offlinefiles
ms.assetid: 3913dc9d-f640-407d-b3b9-77b33f26e726
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOfflineFilesDirtyInfo interface [Offline Files],RemoteDirtyByteCount method, IOfflineFilesDirtyInfo.RemoteDirtyByteCount, IOfflineFilesDirtyInfo::RemoteDirtyByteCount, RemoteDirtyByteCount, RemoteDirtyByteCount method [Offline Files], RemoteDirtyByteCount method [Offline Files],IOfflineFilesDirtyInfo interface, cscobj/IOfflineFilesDirtyInfo::RemoteDirtyByteCount, of.iofflinefilesdirtyinfo_remotedirtybytecount
ms.topic: method
f1_keywords: ["cscobj/IOfflineFilesDirtyInfo.RemoteDirtyByteCount"]
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista with SP1
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
 - IOfflineFilesDirtyInfo.RemoteDirtyByteCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOfflineFilesDirtyInfo::RemoteDirtyByteCount


## -description


This method is reserved for future use.


## -parameters




### -param pDirtyByteCount [out]

The number of bytes of unsynchronized data.


## -returns



Returns <b>S_OK</b> if successful, or an error value otherwise.




## -remarks



This method can only be called for file items, which are represented by <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/nn-cscobj-iofflinefilesfileitem">IOfflineFilesFileItem</a> objects.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/nn-cscobj-iofflinefilesdirtyinfo">IOfflineFilesDirtyInfo</a>
 

 

