---
UID: NF:faxcomex.IFaxOutgoingJob.Refresh
title: IFaxOutgoingJob::Refresh
author: windows-sdk-content
description: The Refresh method refreshes FaxOutgoingJob object information from the fax server.
old-location: fax\_mfax_faxoutgoingjob_cpp_mfax_faxoutgoingjob_refresh_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_2oq0.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxOutgoingJob interface [Fax Service],Refresh method, IFaxOutgoingJob.Refresh, IFaxOutgoingJob::Refresh, Refresh, Refresh method [Fax Service], Refresh method [Fax Service],IFaxOutgoingJob interface, _mfax_faxoutgoingjob.refresh, fax._mfax_faxoutgoingjob_cpp_mfax_faxoutgoingjob_refresh_cpp, fax._mfax_faxoutgoingjob_refresh, faxcomex/IFaxOutgoingJob::Refresh
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
 - IFaxOutgoingJob.Refresh
 - IFaxOutgoingJob.Refresh
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutgoingJob::Refresh


## -description


The Refresh method refreshes <a href="https://msdn.microsoft.com/en-us/library/ms689115(v=VS.85).aspx">FaxOutgoingJob</a> object information from the fax server.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To use this method, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farSUBMIT_LOW</a> or <b>farQUERY_JOBS</b> access right.

With the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farSUBMIT_LOW</a> access right, users will be able to use this method only for their own faxes. With the <b>farQUERY_JOBS</b> access right, users will be able to use this method for all faxes on the server.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms689115(v=VS.85).aspx">FaxOutgoingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms689116(v=VS.85).aspx">IFaxOutgoingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693393(v=VS.85).aspx">Visual Basic Example</a>
 

 

