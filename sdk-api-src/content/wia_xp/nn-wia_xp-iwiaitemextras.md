---
UID: NN:wia_xp.IWiaItemExtras
title: IWiaItemExtras (wia_xp.h)
author: windows-sdk-content
description: The IWiaItemExtras interface provides several methods that enable applications to communicate with hardware drivers.
old-location: wia\_wia_IWiaItemExtras.htm
tech.root: wia
ms.assetid: VS|wia|~\wia\refwia\ifaces\iwiaitemextras\iwiaitemextras.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWiaItemExtras, IWiaItemExtras interface [WIA], IWiaItemExtras interface [WIA],described, _wia_IWiaItemExtras, wia._wia_IWiaItemExtras, wia_xp/IWiaItemExtras
ms.topic: interface
req.header: wia_xp.h
req.include-header: Wia.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
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
req.lib: Wiaguid.lib
req.dll: Wiaservc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wiaservc.dll
api_name:
 - IWiaItemExtras
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWiaItemExtras interface


## -description


The <b>IWiaItemExtras</b> interface provides several methods that enable applications to communicate with hardware drivers.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWiaItemExtras</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWiaItemExtras</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWiaItemExtras</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms629970(v=VS.85).aspx">CancelPendingIO</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms629970(v=VS.85).aspx">IWiaItemExtras::CancelPendingIO</a> method cancels all pending input/output operations on the driver.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms629973(v=VS.85).aspx">Escape</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms629973(v=VS.85).aspx">IWiaItemExtras::Escape</a> method sends a request for a vendor-specific I/O operation to a still image device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms629974(v=VS.85).aspx">GetExtendedErrorInfo</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/en-us/library/ms629974(v=VS.85).aspx">IWiaItemExtras::GetExtendedErrorInfo</a> method gets a string from the device driver that contains information about the most recent error. Call this method after an error during an operation on a WIA item (such as data transfer).

</td>
</tr>
</table> 


## -remarks



The <b>IWiaItemExtras</b> interface, like all Component Object Model (COM) interfaces, inherits the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface methods. 

<table class="clsStd">
<tr>
<th>IUnknown Methods</th>
<th>Description</th>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">IUnknown::QueryInterface</a>
</td>
<td>Returns pointers to supported interfaces.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/b4316efd-73d4-4995-b898-8025a316ba63">IUnknown::AddRef</a>
</td>
<td>Increments reference count.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">IUnknown::Release</a>
</td>
<td>Decrements reference count.</td>
</tr>
</table>
 



