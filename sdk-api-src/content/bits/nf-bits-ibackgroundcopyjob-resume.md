---
UID: NF:bits.IBackgroundCopyJob.Resume
title: IBackgroundCopyJob::Resume (bits.h)
author: windows-sdk-content
description: Activates a new job or restarts a job that has been suspended.
old-location: bits\ibackgroundcopyjob_resume.htm
tech.root: Bits
ms.assetid: a9e6f057-0a51-4f2d-810b-edbb3e019370
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IBackgroundCopyJob interface [BITS],Resume method, IBackgroundCopyJob.Resume, IBackgroundCopyJob::Resume, Resume, Resume method [BITS], Resume method [BITS],IBackgroundCopyJob interface, _drz_ibackgroundcopyjob_resume, bits.ibackgroundcopyjob_resume, bits/IBackgroundCopyJob::Resume
ms.topic: method
req.header: bits.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Bits.lib
req.dll: QmgrPrxy.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - QmgrPrxy.dll
api_name:
 - IBackgroundCopyJob.Resume
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBackgroundCopyJob::Resume


## -description


Activates a new job or restarts a job that has been suspended.


## -parameters






## -returns



This method returns the following <b>HRESULT</b> values, as well as others.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>S_OK</b></b></dt>
</dl>
</td>
<td width="60%">
Job was successfully restarted.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>BG_E_EMPTY</b></dt>
</dl>
</td>
<td width="60%">
There are no files to transfer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>BG_E_INVALID_STATE</b></dt>
</dl>
</td>
<td width="60%">
The state of the job cannot be BG_JOB_STATE_CANCELLED or BG_JOB_STATE_ACKNOWLEDGED.

</td>
</tr>
</table>
 




## -remarks



When you create a job, the job is initially suspended. Calling <b>Resume</b> moves the job from the suspended state to the queued state. The job stays in the queued state until the scheduler determines it is the job's turn to transfer files. Note that the job must contain one or more files before calling this method. If the job is of type BG_JOB_TYPE_UPLOAD_REPLY and you want to specify the name of the reply file, you should call the 
<a href="https://msdn.microsoft.com/9f8591a3-ecc2-497a-ac12-67e5862efde4">IBackgroundCopyJob2::SetReplyFileName</a> method before calling 
<b>Resume</b>.

If a job that is in the BG_JOB_STATE_TRANSIENT_ERROR or BG_JOB_STATE_ERROR state, call the 
<b>Resume</b> method to restart the job after you fix the error.




## -see-also




<a href="https://msdn.microsoft.com/bb3f32d9-298a-4099-8d87-4057ddefb0ba">IBackgroundCopyJob::Cancel</a>



<a href="https://msdn.microsoft.com/88429730-b8e5-4969-934c-f0945fdd46a6">IBackgroundCopyJob::Suspend</a>
 

 

