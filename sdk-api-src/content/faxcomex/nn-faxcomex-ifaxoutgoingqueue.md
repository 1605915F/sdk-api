---
UID: NN:faxcomex.IFaxOutgoingQueue
title: IFaxOutgoingQueue
author: windows-sdk-content
description: The IFaxOutgoingQueue interface defines a FaxOutgoingQueue configuration object used by a fax client application to set and retrieve the configuration parameters on the outbound fax queue on a fax server.
old-location: fax\_mfax_faxoutgoingqueue_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_0dyd_cpp.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxOutgoingQueue, IFaxOutgoingQueue interface [Fax Service], IFaxOutgoingQueue interface [Fax Service],described, _mfax_faxoutgoingqueue_cpp, fax._mfax_faxoutgoingqueue_cpp, faxcomex/IFaxOutgoingQueue
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
 - IFaxOutgoingQueue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutgoingQueue interface


## -description


The <b>IFaxOutgoingQueue</b> interface defines a <a href="https://msdn.microsoft.com/en-us/library/ms687528(v=VS.85).aspx">FaxOutgoingQueue</a> configuration object used by a fax client application to set and retrieve the configuration parameters on the outbound fax queue on a fax server. 


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFaxOutgoingQueue</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IFaxOutgoingQueue</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>IFaxOutgoingQueue</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms688625(v=VS.85).aspx">GetJob</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms688625(v=VS.85).aspx">IFaxOutgoingQueue::GetJob</a> method returns an outbound fax job in the job queue according to its ID.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms690178(v=VS.85).aspx">GetJobs</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms690178(v=VS.85).aspx">IFaxOutgoingQueue::GetJobs</a> method returns a collection of the outbound fax jobs in the job queue.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms689117(v=VS.85).aspx">Refresh</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689117(v=VS.85).aspx">IFaxOutgoingQueue::Refresh</a> method refreshes <a href="https://msdn.microsoft.com/en-us/library/ms687528(v=VS.85).aspx">FaxOutgoingQueue</a> object information from the fax server. When the <b>IFaxOutgoingQueue::Refresh</b> method is called, any configuration changes made after the last <a href="https://msdn.microsoft.com/en-us/library/ms689100(v=VS.85).aspx">IFaxOutgoingQueue::Save</a> method call are lost.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms689100(v=VS.85).aspx">Save</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689100(v=VS.85).aspx">IFaxOutgoingQueue::Save</a> method saves the <a href="https://msdn.microsoft.com/en-us/library/ms687528(v=VS.85).aspx">FaxOutgoingQueue</a> object data.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFaxOutgoingQueue</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689606(v=VS.85).aspx">AgeLimit</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689606(v=VS.85).aspx">IFaxOutgoingQueue::get_AgeLimit</a> property is a value that indicates the number of days that the fax service retains an unsent job in the fax job queue. 

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689158(v=VS.85).aspx">AllowPersonalCoverPages</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The AllowPersonalCoverPages property is a Boolean value that indicates whether fax client applications can include a user-designed cover page with fax transmissions.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689147(v=VS.85).aspx">Blocked</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689147(v=VS.85).aspx">IFaxOutgoingQueue::get_Blocked</a> property is a Boolean value that indicates whether the job queue for outgoing faxes is blocked. 

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms690067(v=VS.85).aspx">Branding</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms690067(v=VS.85).aspx">IFaxOutgoingQueue::get_Branding</a> property is a Boolean value that indicates whether the fax service generates a brand (banner) at the top of outgoing fax transmissions. A brand contains transmission-related information, such as the transmitting station identifier, date, time, and page count.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689070(v=VS.85).aspx">DiscountRateEnd</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689070(v=VS.85).aspx">IFaxOutgoingQueue::get_DiscountRateEnd</a> property is a value that indicates the time at which the discount period for transmitting faxes ends. The discount period applies to outgoing faxes.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689570(v=VS.85).aspx">DiscountRateStart</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689570(v=VS.85).aspx">IFaxOutgoingQueue::get_DiscountRateStart</a> property is a value that indicates the time at which the discount period for transmitting faxes begins. The discount period applies to outgoing faxes.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms690048(v=VS.85).aspx">Paused</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms690048(v=VS.85).aspx">IFaxOutgoingQueue::get_Paused</a> property is a Boolean value that indicates whether the job queue for outgoing faxes is paused. 

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms690191(v=VS.85).aspx">Retries</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms690191(v=VS.85).aspx">IFaxOutgoingQueue::get_Retries</a> property is a value that indicates the number of times that the fax service attempts to retransmit an outgoing fax when the initial transmission fails.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689088(v=VS.85).aspx">RetryDelay</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689088(v=VS.85).aspx">IFaxOutgoingQueue::get_RetryDelay</a> property is a value that indicates the time interval, in minutes, that the fax service waits before attempting to retransmit an outbound fax job.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/en-us/library/ms689568(v=VS.85).aspx">UseDeviceTSID</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms689568(v=VS.85).aspx">IFaxOutgoingQueue::get_UseDeviceTSID</a> property is a Boolean value that indicates whether the fax service uses the device TSID instead of a sender TSID. 

</td>
</tr>
</table> 


## -remarks



A default implementation of <b>IFaxOutgoingQueue</b> is provided as the <a href="https://msdn.microsoft.com/en-us/library/ms687528(v=VS.85).aspx">FaxOutgoingQueue</a> object. 



