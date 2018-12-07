---
UID: NN:uiautomationclient.IUIAutomation6
title: IUIAutomation6
author: windows-sdk-content
description: Extends the IUIAutomation5 interface to expose additional methods for controlling Microsoft UI Automation functionality.
old-location: winauto\uiauto_IUIAutomation6.htm
tech.root: WinAuto
ms.assetid: FA42D0D0-E6D6-41C6-BCF1-6F9C02D2BE1D
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUIAutomation6, IUIAutomation6 interface [Windows Accessibility], IUIAutomation6 interface [Windows Accessibility],described, uiautomationclient/IUIAutomation6, winauto.uiauto_IUIAutomation6
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: uiautomationclient.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1809 [desktop apps only]
req.target-min-winversvr: Windows Server, version 1709 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationClient.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: UIAutomationCore.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - UIAutomationCore.dll
api_name:
 - IUIAutomation6
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAutomation6 interface


## -description


Extends the <a href="https://msdn.microsoft.com/BCF67DB0-DF5B-4CED-9C32-01F126494129">IUIAutomation5</a> interface to expose additional methods for controlling Microsoft UI Automation functionality.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IUIAutomation6</b> interface inherits from <a href="https://msdn.microsoft.com/BCF67DB0-DF5B-4CED-9C32-01F126494129">IUIAutomation5</a>. <b>IUIAutomation6</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>IUIAutomation6</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/05D46393-6B76-415A-A1F9-F28B5DAF2074">AddActiveTextPositionChangedEventHandler</a>
</td>
<td align="left" width="63%">
Registers a method that handles when the active text position changes.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/8F131A7C-BC03-4967-9ED8-624086DEA112">AddEventHandlerGroup</a>
</td>
<td align="left" width="63%">
Registers a collection of event handler methods specified with the <a href="https://docs.microsoft.com/windows/desktop/api/uiautomationclient/nf-uiautomationclient-iuiautomation6-createeventhandlergroup">CreateEventHandlerGroup</a>.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="winauto.uauto_iuiautomation6_createeventhandlergroup">CreateEventHandlerGroup</a>
</td>
<td align="left" width="63%">
 Registers one or more event listeners in a single method call.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/92A6E9BA-0B68-4890-90EE-16F4B0929340">RemoveActiveTextPositionChangedEventHandler</a>
</td>
<td align="left" width="63%">
Removes an active text position changed event handler.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/43BDE7F5-67DF-4DE5-AEDE-068421375E07">RemoveEventHandlerGroup</a>
</td>
<td align="left" width="63%">
Asynchronously removes the specified UI Automation event handler group.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IUIAutomation6</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/44BBBE06-6A41-4DE7-8C1B-E277D3FCB545">CoalesceEvents</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
Gets or sets whether an accessible technology client receives all events, or a subset where duplicate events are detected and filtered.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/09184E02-1007-4F49-8B03-97430CD6327E">ConnectionRecoveryBehavior</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
Indicates whether an accessible technology client adjusts provider request timeouts when the provider is non-responsive.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/BCF67DB0-DF5B-4CED-9C32-01F126494129">IUIAutomation5</a>



<a href="https://msdn.microsoft.com/dd7cdcf1-3511-424f-b729-b71a7e11cdd8">UI Automation Element Interfaces for Clients</a>
 

 

