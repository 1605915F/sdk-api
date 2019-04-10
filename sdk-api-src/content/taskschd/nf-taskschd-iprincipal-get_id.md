---
UID: NF:taskschd.IPrincipal.get_Id
title: IPrincipal::get_Id (taskschd.h)
author: windows-sdk-content
description: Gets or sets the identifier of the principal.
old-location: taskschd\iprincipal_id.htm
tech.root: taskschd
ms.assetid: 70c31ea8-508a-4971-b62a-b94e87a8857d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IPrincipal interface [Task Scheduler],Id property, IPrincipal.Id, IPrincipal.get_Id, IPrincipal::Id, IPrincipal::get_Id, IPrincipal::put_Id, Id property [Task Scheduler], Id property [Task Scheduler],IPrincipal interface, get_Id, taskschd.iprincipal_id, taskschd/IPrincipal::Id, taskschd/IPrincipal::get_Id, taskschd/IPrincipal::put_Id
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
 - IPrincipal.Id
 - IPrincipal.get_Id
 - IPrincipal.put_Id
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPrincipal::get_Id


## -description


Gets or sets the identifier of the principal.

This property is read/write.


## -parameters


## -remarks



This identifier is also used when specifying the  <a href="https://msdn.microsoft.com/e365955e-1648-4e11-b602-016dcbeb129e">IActionCollection::Context</a> property.

When reading or writing XML for a task, the identifier of the principal is specified in the Id attribute of the <a href="https://msdn.microsoft.com/4ba65976-98d2-4329-80f0-566fac2e9fda">Principal</a> element of the Task Scheduler schema.




## -see-also




<a href="https://msdn.microsoft.com/e365955e-1648-4e11-b602-016dcbeb129e">IActionCollection.Context</a>



<a href="https://msdn.microsoft.com/7aa22af2-7f0a-41c1-89c6-d813780e89bf">IPrincipal</a>



<a href="https://msdn.microsoft.com/15970a51-c139-48b8-b82b-605728d0f386">Task Scheduler</a>
 

 

