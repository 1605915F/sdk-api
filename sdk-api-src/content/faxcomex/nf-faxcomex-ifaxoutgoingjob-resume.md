---
UID: NF:faxcomex.IFaxOutgoingJob.Resume
title: IFaxOutgoingJob::Resume (faxcomex.h)
author: windows-sdk-content
description: The IFaxOutgoingJob::Resume method resumes the paused outbound fax job.
old-location: fax\_mfax_faxoutgoingjob_cpp_mfax_faxoutgoingjob_resume_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_6bs5.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IFaxOutgoingJob interface [Fax Service],Resume method, IFaxOutgoingJob.Resume, IFaxOutgoingJob::Resume, Resume, Resume method [Fax Service], Resume method [Fax Service],IFaxOutgoingJob interface, _mfax_faxoutgoingjob.resume, fax._mfax_faxoutgoingjob_cpp_mfax_faxoutgoingjob_resume_cpp, fax._mfax_faxoutgoingjob_resume, faxcomex/IFaxOutgoingJob::Resume
ms.topic: method
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxOutgoingJob.Resume
 - IFaxOutgoingJob.Resume
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutgoingJob::Resume


## -description


The <b>IFaxOutgoingJob::Resume</b> method resumes the paused outbound fax job.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To use this method, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farSUBMIT_LOW</a> or <b>farMANAGE_JOBS</b> access right. With the <b>farSUBMIT_LOW</b> access right, users will be able to use this method only for their own faxes. With the <b>farMANAGE_JOBS</b> access right, users will be able to use this method for all faxes on the server.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms689115(v=VS.85).aspx">FaxOutgoingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms689116(v=VS.85).aspx">IFaxOutgoingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693393(v=VS.85).aspx">Visual Basic Example</a>
 

 

