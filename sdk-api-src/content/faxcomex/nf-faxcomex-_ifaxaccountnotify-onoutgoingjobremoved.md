---
UID: NF:faxcomex._IFaxAccountNotify.OnOutgoingJobRemoved
title: "_IFaxAccountNotify::OnOutgoingJobRemoved"
author: windows-sdk-content
description: Called by the fax service when an outgoing fax job is removed from the job queue of a particular fax account.
old-location: fax\_mfax_ifaxaccountnotify_onoutgoingjobremoved.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\reference\serviceextendedcom\i\ifaxaccountnotify\onoutgoingjobremoved.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxAccountNotify.OnOutgoingJobRemoved, OnOutgoingJobRemoved, OnOutgoingJobRemoved method [Fax Service], OnOutgoingJobRemoved method [Fax Service],_IFaxAccountNotify interface, _IFaxAccountNotify interface [Fax Service],OnOutgoingJobRemoved method, _IFaxAccountNotify.OnOutgoingJobRemoved, _IFaxAccountNotify::OnOutgoingJobRemoved, _mfax_ifaxaccountnotify_onoutgoingjobremoved, fax._mfax_ifaxaccountnotify_onoutgoingjobremoved, faxcomex/_IFaxAccountNotify::OnOutgoingJobRemoved
ms.topic: method
req.header: faxcomex.h
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
 - _IFaxAccountNotify.OnOutgoingJobRemoved
 - IFaxAccountNotify.OnOutgoingJobRemoved
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# _IFaxAccountNotify::OnOutgoingJobRemoved


## -description


Called by the fax service when an outgoing fax job is removed from the job queue of a particular fax account.


## -parameters




### -param pFaxAccount [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa359058(v=VS.85).aspx">IFaxAccount</a>*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Aa359058(v=VS.85).aspx">IFaxAccount</a> object.


### -param bstrJobId [in]

Type: <b>BSTR</b>

Null-terminated string that contains the ID of the job removed from the job queue.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To implement this functionality in Visual Basic, select and implement the appropriate event procedure. 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa359031(v=VS.85).aspx">IFaxAccountNotify</a>
 

 

