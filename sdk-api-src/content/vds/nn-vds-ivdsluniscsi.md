---
UID: NN:vds.IVdsLunIscsi
title: IVdsLunIscsi
author: windows-sdk-content
description: Provides methods for performing query and configuration operations on an iSCSI LUN.
old-location: base\ivdsluniscsi.htm
tech.root: vds
ms.assetid: 5b1e6204-6cc0-4d94-8e54-fa963f83ae39
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsLunIscsi, IVdsLunIscsi interface [VDS], IVdsLunIscsi interface [VDS],described, base.ivdsluniscsi, vds/IVdsLunIscsi, vdshwprv/IVdsLunIscsi
ms.topic: interface
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Vds.h
 - VdsHwPrv.h
api_name:
 - IVdsLunIscsi
product: Windows
targetos: Windows
req.typenames: 
req.redist: VDS 1.1
---

# IVdsLunIscsi interface


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Provides 
   methods for performing query and configuration operations on an iSCSI LUN.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVdsLunIscsi</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IVdsLunIscsi</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVdsLunIscsi</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/eb80020b-caf8-4d85-b250-d9a8738b8848">AssociateTargets</a>
</td>
<td align="left" width="63%">
Associates LUNs with subsystem iSCSI targets.</p> (Inherited from <b>IVdsLunIscsi</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4979e3c1-d966-4dfd-bb87-73c3e1252c50">QueryAssociatedTargets</a>
</td>
<td align="left" width="63%">
Returns an enumeration of currently associated iSCSI targets—the targets 
   through which the LUN is accessible.</p> (Inherited from <b>IVdsLunIscsi</b>)</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/0bddfd62-881d-4fda-b303-ed38d434af55">VDS Interfaces</a>
 

 

