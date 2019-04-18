---
UID: NF:pla.IDataManager.get_MaxSize
title: IDataManager::get_MaxSize (pla.h)
author: windows-sdk-content
description: Retrieves or sets the maximum disk space to be used by all data collectors in the set.
old-location: pla\idatamanager_maxsize.htm
tech.root: PLA
ms.assetid: a9508617-acb5-4e11-8f4a-72c8e5cb4cba
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IDataManager interface [PLA],MaxSize property, IDataManager.MaxSize, IDataManager.get_MaxSize, IDataManager::MaxSize, IDataManager::get_MaxSize, IDataManager::put_MaxSize, MaxSize property [PLA], MaxSize property [PLA],IDataManager interface, base.idatamanager_maxsize, get_MaxSize, pla.idatamanager_maxsize, pla/IDataManager::MaxSize, pla/IDataManager::get_MaxSize, pla/IDataManager::put_MaxSize
ms.topic: method
req.header: pla.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: Pla.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Pla.dll
api_name:
 - IDataManager.MaxSize
 - IDataManager.get_MaxSize
 - IDataManager.put_MaxSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDataManager::get_MaxSize


## -description


Retrieves or sets the maximum disk space to be used by all data collectors in the set. 

This property is read/write.


## -parameters


## -remarks



The maximum value applies to all files in all subfolders under the path specified by the <a href="https://msdn.microsoft.com/42940cec-c76a-433c-9308-f030dacb05a4">IDataCollectorSet::RootPath</a> property. 

This value is used by the data manager:

<ul>
<li>Before the data collector set starts if the value of the <a href="https://msdn.microsoft.com/23c7aced-d159-4d5e-a9ff-f0ca5b3e4470">IDataManager::CheckBeforeRunning</a> property is VARIANT_TRUE. If the maximum size is exceeded, the manager prevents the data collector set from running.</li>
<li>After the collection is completed. If the maximum size is exceeded, the data manager will start deleting folders (according to the <a href="https://msdn.microsoft.com/541cd28c-2e01-4b8a-9cd3-044896c8fb80">IDataManager::ResourcePolicy</a> property) until the total size is below the maximum size.</li>
</ul>
The maximum size value is ignored for performance counter log collection. To work around this issue, you can do one of two things:

<ul>
<li>Set the <a href="https://msdn.microsoft.com/d1b35b02-cfda-42a4-bd1d-d837a91861d6">IDataCollector::LogCircular</a> property to <b>True</b> and set the <a href="https://msdn.microsoft.com/7dd96822-a398-42c3-94f1-b9cd7a647575">IDataCollectorSet::SegmentMaxSize</a> property to the desired maximum size.</li>
<li>Set the <a href="https://msdn.microsoft.com/d1b35b02-cfda-42a4-bd1d-d837a91861d6">IDataCollector::LogCircular</a> property to <b>False</b>, set the <a href="https://msdn.microsoft.com/7dd96822-a398-42c3-94f1-b9cd7a647575">IDataCollectorSet::SegmentMaxSize</a> property equal to the maximum folder size, and set the <a href="https://msdn.microsoft.com/5ecac3dd-0cd1-4563-a6b3-1b98e29fe769">IDataCollectorSet::Segment</a> property to <b>False</b>.</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/a153d88f-4c7e-45fd-9cd8-497160711de4">IDataManager</a>
 

 

