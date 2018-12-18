---
UID: NN:imapi2.IWriteEngine2EventArgs
title: IWriteEngine2EventArgs
author: windows-sdk-content
description: Use this interface to retrieve information about the current write operation. This interface is passed to the DWriteEngine2Events::Update method that you implement.
old-location: imapi\iwriteengine2eventargs.htm
tech.root: imapi
ms.assetid: 1922410a-5871-477f-b778-36b12ad95168
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWriteEngine2EventArgs, IWriteEngine2EventArgs interface [IMAPI], IWriteEngine2EventArgs interface [IMAPI],described, imapi.iwriteengine2eventargs, imapi2/IWriteEngine2EventArgs
ms.topic: interface
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - imapi2.h
api_name:
 - IWriteEngine2EventArgs
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWriteEngine2EventArgs interface


## -description


Use this interface to retrieve information about the current write operation. This interface is passed to the <a href="https://msdn.microsoft.com/efee838d-aa6e-41a0-aafb-64ba6ca19f29">DWriteEngine2Events::Update</a> method that you implement.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWriteEngine2EventArgs</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IWriteEngine2EventArgs</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWriteEngine2EventArgs</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d62eeb31-cf47-4456-832c-9a29c045b11c">get_FreeSystemBuffer</a>
</td>
<td align="left" width="63%">
Retrieves the number of unused bytes in the internal data buffer that is used for writing to disc.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2db929b4-dbba-4f6a-bde0-0cefb30abf64">get_LastReadLba</a>
</td>
<td align="left" width="63%">
Retrieves the address of the sector most recently read from the burn image.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ccb964b5-dd6f-4250-b6d2-41154258872f">get_LastWrittenLba</a>
</td>
<td align="left" width="63%">
Retrieves the address of the sector most recently written to the device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b23c81c2-792e-45fc-b862-6daf5b1a6fd1">get_SectorCount</a>
</td>
<td align="left" width="63%">
Retrieves the number of sectors to write to the device in the current write operation.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1c2d1a1f-04b7-4453-af52-4f96e5536ad2">get_StartLba</a>
</td>
<td align="left" width="63%">
Retrieves the starting logical block address (LBA) of the current write operation.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/dfdf4116-0402-4c90-8b9b-0758fd0bb973">get_TotalSystemBuffer</a>
</td>
<td align="left" width="63%">
Retrieves the size of the internal data buffer that is used for writing to disc.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/905c476f-33cd-4eda-a342-c7a20479d63c">get_UsedSystemBuffer</a>
</td>
<td align="left" width="63%">
Retrieves the number of used bytes in the internal data buffer that is used for writing to disc.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/697f8247-6940-4b5e-8521-df89838837be">DWriteEngine2Events</a>
 

 

