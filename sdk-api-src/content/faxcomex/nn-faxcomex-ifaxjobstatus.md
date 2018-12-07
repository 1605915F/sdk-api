---
UID: NN:faxcomex.IFaxJobStatus
title: IFaxJobStatus
author: windows-sdk-content
description: The IFaxJobStatus interface is used for notifications and to hold the dynamic information of the job.
old-location: fax\_mfax_faxjobstatus_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_3p6b_cpp.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxJobStatus, IFaxJobStatus interface [Fax Service], IFaxJobStatus interface [Fax Service],described, _mfax_faxjobstatus_cpp, fax._mfax_faxjobstatus_cpp, faxcomex/IFaxJobStatus
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
 - IFaxJobStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxJobStatus interface


## -description


The <b>IFaxJobStatus</b> interface is used for notifications and to hold the dynamic information of the job. Dynamic information is data that changes as a job progresses. This may include the current job status, the page that is currently being transmitted, and the number of attempts the fax service has made to transmit the job (retries). The fax service uses this object to notify a fax client application of job updates. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms693448(v=VS.85).aspx">Fax Job Status</a>.


## -remarks



You do not create the <a href="https://msdn.microsoft.com/en-us/library/ms685964(v=VS.85).aspx">FaxJobStatus</a> object. It is received as part of a notification when you implement <a href="https://msdn.microsoft.com/en-us/library/ms688427(v=VS.85).aspx">IFaxServerNotify::OnIncomingJobChanged</a> or <a href="https://msdn.microsoft.com/en-us/library/ms688641(v=VS.85).aspx">IFaxServerNotify::OnOutgoingJobChanged</a>, which include a parameter of the type <b>FaxJobStatus</b>. When the event occurs and the implemented function is called, you receive this object containing the dynamic information.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms685964(v=VS.85).aspx">FaxJobStatus</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

