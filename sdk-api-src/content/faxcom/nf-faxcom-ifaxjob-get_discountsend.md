---
UID: NF:faxcom.IFaxJob.get_DiscountSend
title: IFaxJob::get_DiscountSend
author: windows-sdk-content
description: The IFaxJob::get_DiscountSend property is a Boolean value that indicates whether the fax server will transmit the fax job during the discount rate period. The discount period applies only to outgoing fax transmissions.
old-location: fax\_mfax_ifaxjob_mfax_ifaxjob_get_discountsend_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_8h9g.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DiscountSend property [Fax Service], DiscountSend property [Fax Service],IFaxJob interface, IFaxJob interface [Fax Service],DiscountSend property, IFaxJob.DiscountSend, IFaxJob.get_DiscountSend, IFaxJob::DiscountSend, IFaxJob::get_DiscountSend, _mfax_ifaxjob_get_discountsend, fax._mfax_ifaxjob_get_discountsend, fax._mfax_ifaxjob_mfax_ifaxjob_get_discountsend_cpp, faxcom/IFaxJob::DiscountSend, faxcom/IFaxJob::get_DiscountSend, get_DiscountSend
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcom.h
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
req.lib: 
req.dll: Faxcom.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Faxcom.dll
api_name:
 - IFaxJob.DiscountSend
 - IFaxJob.get_DiscountSend
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxJob::get_DiscountSend


## -description


The <b>IFaxJob::get_DiscountSend</b> property is a Boolean value that indicates whether the fax server will transmit the fax job during the discount rate period. The discount period applies only to outgoing fax transmissions. 

This property is read-only.


## -parameters


## -remarks



To determine the period during which the discount rate applies, you can use the following IFaxServer properties. 

<ul>
<li>
<a href="https://msdn.microsoft.com/98355801-ad54-4b1e-a2f2-dcd22ede26e2">DiscountRateStartMinute</a>
</li>
<li>
<a href="https://msdn.microsoft.com/a8e1bf04-7fc4-48b3-8682-b06c550122a7">DiscountRateEndMinute</a>
</li>
<li>
<a href="https://msdn.microsoft.com/b144d4db-bd0e-4198-8653-6b22013c3d2e">DiscountRateStartHour</a>
</li>
<li>
<a href="https://msdn.microsoft.com/959f2960-2e42-485e-9791-53849166bf88">DiscountRateEndHour</a>
</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692310(v=VS.85).aspx">IFaxJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692372(v=VS.85).aspx">IFaxJobs</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691821(v=VS.85).aspx">Managing Fax Jobs</a>
 

 

