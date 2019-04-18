---
UID: NF:mstask.ITaskTrigger.SetTrigger
title: ITaskTrigger::SetTrigger (mstask.h)
author: windows-sdk-content
description: The SetTrigger method sets the trigger criteria for a task trigger.
old-location: taskschd\itasktrigger_settrigger.htm
tech.root: taskschd
ms.assetid: 2f445835-a409-4a03-b853-4e0b07ded1ea
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITaskTrigger interface [Task Scheduler],SetTrigger method, ITaskTrigger.SetTrigger, ITaskTrigger::SetTrigger, SetTrigger, SetTrigger method [Task Scheduler], SetTrigger method [Task Scheduler],ITaskTrigger interface, _msb_itasktrigger_settrigger, mstask/ITaskTrigger::SetTrigger, taskschd.itasktrigger_settrigger
ms.topic: method
req.header: mstask.h
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
req.lib: Mstask.lib
req.dll: Mstask.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mstask.dll
api_name:
 - ITaskTrigger.SetTrigger
product: Windows
targetos: Windows
req.typenames: 
req.redist: Internet Explorer 4.0 or later on Windows NT 4.0 and Windows 95
ms.custom: 19H1
---

# ITaskTrigger::SetTrigger


## -description


<p class="CCE_Message">[[This API may be altered or unavailable in subsequent versions of the operating system or product. Please use the <a href="https://msdn.microsoft.com/67ed58e1-e54c-4c02-a6c4-d9ab8dc0f83e">Task Scheduler 2.0 Interfaces</a> instead.] ]

The 
<b>SetTrigger</b> method sets the trigger criteria for a task <a href="https://msdn.microsoft.com/en-us/library/Aa382533(v=VS.85).aspx">trigger</a>.


## -parameters




### -param pTrigger [in]

A pointer to a 
<a href="https://msdn.microsoft.com/b4716e32-7c7a-40ab-baa1-4c7ebafc3d71">TASK_TRIGGER</a> structure that contains the values that define the new task trigger.


## -returns



The 
<b>SetTrigger</b> method returns one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The operation was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The arguments are not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Not enough memory is available.

</td>
</tr>
</table>
 




## -remarks



The <b>wBeginDay</b>, <b>wBeginMonth</b>, and <b>wBeginYear</b> members of the 
<a href="https://msdn.microsoft.com/b4716e32-7c7a-40ab-baa1-4c7ebafc3d71">TASK_TRIGGER</a> structure must be set to a valid day, month, and year respectively.

A task can have any number of triggers associated with it. The times that the task will run are the union of all the triggers defined for that task.

To update the task with these new trigger settings, applications must call the 
<a href="https://msdn.microsoft.com/en-us/library/ms693701(v=VS.85).aspx">IPersistFile::Save</a> method after calling 
<b>SetTrigger</b>.


#### Examples

The following code shows the variable declaration and calling syntax for this method, including the required members of 
<a href="https://msdn.microsoft.com/b4716e32-7c7a-40ab-baa1-4c7ebafc3d71">TASK_TRIGGER</a>. Setting the trigger criteria when creating a new trigger, see <a href="https://msdn.microsoft.com/c0f121ff-d0a5-4b6c-935c-6f47b4ea26d5">Creating a New Trigger</a>.


```cpp
HRESULT hr = S_OK;

TASK_TRIGGER Trigger;

ZeroMemory(&Trigger, sizeof(TASK_TRIGGER));

Trigger.cbTriggerSize = sizeof(TASK_TRIGGER);
Trigger.wBeginDay = 1;
Trigger.wBeginMonth = 1;
Trigger.wBeginYear = 1999;

// pITaskTrigger is a previously assigned ITaskTrigger pointer.
hr = pITaskTrigger->SetTrigger(&Trigger);
if (FAILED(hr))
{
   printf("Failed SetTrigger\n");
   exit(1);
}

```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms693701(v=VS.85).aspx">IPersistFile::Save</a>



<a href="https://msdn.microsoft.com/990702f4-fb6f-47a7-b538-f6632f831a4e">ITaskTrigger</a>



<a href="https://msdn.microsoft.com/d6c9110d-c79e-475d-871b-83dca6577fc5">ITaskTrigger::GetTrigger</a>



<a href="https://msdn.microsoft.com/b4716e32-7c7a-40ab-baa1-4c7ebafc3d71">TASK_TRIGGER</a>
 

 

