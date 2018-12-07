---
UID: NN:vds.IVdsRemovable
title: IVdsRemovable
author: windows-sdk-content
description: Provides methods to query and eject a removable disk, such as a CD-ROM.
old-location: base\ivdsremovable.htm
tech.root: vds
ms.assetid: 86dcd76a-0de0-42f4-9360-87cf7ca4ebf6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsRemovable, IVdsRemovable interface [VDS], IVdsRemovable interface [VDS],described, base.ivdsremovable, vds/IVdsRemovable
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: Uuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Uuid.lib
 - Uuid.dll
api_name:
 - IVdsRemovable
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsRemovable interface


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Provides methods to query and eject a removable disk, such as a CD-ROM.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVdsRemovable</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IVdsRemovable</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVdsRemovable</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c77885bd-67af-41c1-9190-e0148c7b7ed5">Eject</a>
</td>
<td align="left" width="63%">
Ejects the media from the current device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6a56be84-ddf3-4c82-9465-4cb683e993f6">QueryMedia</a>
</td>
<td align="left" width="63%">
Returns the details of the media in a removable disk or CD-ROM/DVD drive.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/65e14273-8127-4667-b5c8-362ad54b4782">Disk Object</a>



<a href="https://msdn.microsoft.com/0bddfd62-881d-4fda-b303-ed38d434af55">VDS Interfaces</a>
 

 

