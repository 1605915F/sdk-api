---
UID: NF:taskschd.IRepetitionPattern.get_Interval
title: IRepetitionPattern::get_Interval (taskschd.h)
author: windows-sdk-content
description: Gets or sets the amount of time between each restart of the task.
old-location: taskschd\irepetitionpattern_interval.htm
tech.root: taskschd
ms.assetid: 3ba8e4b8-c0f9-4b73-8351-b1c1b32a1e39
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IRepetitionPattern interface [Task Scheduler],Interval property, IRepetitionPattern.Interval, IRepetitionPattern.get_Interval, IRepetitionPattern::Interval, IRepetitionPattern::get_Interval, IRepetitionPattern::put_Interval, Interval property [Task Scheduler], Interval property [Task Scheduler],IRepetitionPattern interface, get_Interval, taskschd.irepetitionpattern_interval, taskschd/IRepetitionPattern::Interval, taskschd/IRepetitionPattern::get_Interval, taskschd/IRepetitionPattern::put_Interval
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
 - IRepetitionPattern.Interval
 - IRepetitionPattern.get_Interval
 - IRepetitionPattern.put_Interval
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRepetitionPattern::get_Interval


## -description


Gets or sets the amount of time between each restart of the task.

This property is read/write.


## -parameters


## -remarks



If you specify a repetition duration for a task, you must also specify the repetition interval.

When reading or writing XML for a task, the repetition interval is specified in the  <a href="https://msdn.microsoft.com/28c6475a-88e3-44ac-92c7-6f463e8460c9">Interval</a> element of the Task Scheduler schema.




## -see-also




<a href="https://msdn.microsoft.com/7eea143b-d2f8-44d2-a3ec-8328a0bc69ef">IRepetitionPattern</a>



<a href="https://msdn.microsoft.com/15970a51-c139-48b8-b82b-605728d0f386">Task Scheduler</a>
 

 

