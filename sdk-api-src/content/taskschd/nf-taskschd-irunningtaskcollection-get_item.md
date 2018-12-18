---
UID: NF:taskschd.IRunningTaskCollection.get_Item
title: IRunningTaskCollection::get_Item
author: windows-sdk-content
description: Gets the specified task from the collection.
old-location: taskschd\irunningtaskcollection_item.htm
tech.root: taskschd
ms.assetid: e82e7e1b-a3bd-4456-85a9-e0005f954618
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IRunningTaskCollection interface [Task Scheduler],Item property, IRunningTaskCollection.Item, IRunningTaskCollection.get_Item, IRunningTaskCollection::Item, IRunningTaskCollection::get_Item, Item property [Task Scheduler], Item property [Task Scheduler],IRunningTaskCollection interface, get_Item, taskschd.irunningtaskcollection_item, taskschd/IRunningTaskCollection::Item, taskschd/IRunningTaskCollection::get_Item
ms.topic: method
req.header: taskschd.h
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
req.lib: Taskschd.lib
req.dll: Taskschd.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - taskschd.dll
api_name:
 - IRunningTaskCollection.Item
 - IRunningTaskCollection.get_Item
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRunningTaskCollection::get_Item


## -description


Gets the specified task from the collection.

This property is read-only.


## -parameters


## -remarks



IRunningTaskCollection::get_Item returns E_INVALIDARG and E_TYPE_MISMATCH instead of E_INVALID_VARIANT when an invalid argument is specified.

Collections are 1-based. That is, the index for the first item in the collection is 1.




## -see-also




<a href="https://msdn.microsoft.com/71a06a8f-8628-415d-b002-977c0d27f9a4">IRunningTask</a>



<a href="https://msdn.microsoft.com/f95efba5-563d-49c0-81d3-143aa158ad8f">IRunningTaskCollection</a>
 

 

