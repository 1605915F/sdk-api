---
UID: NN:vdshwprv.IVdsAsync
title: IVdsAsync
author: windows-sdk-content
description: Manages asynchronous operations. Methods that initiate asynchronous operations return a pointer to an IVdsAsync interface, allowing the caller to optionally cancel, wait for, or query the status of the asynchronous operation.
old-location: base\ivdsasync.htm
tech.root: vds
ms.assetid: 7814b8ef-84b4-453e-b480-c32b67e5af93
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsAsync, IVdsAsync interface [VDS], IVdsAsync interface [VDS],described, base.ivdsasync, vds/IVdsAsync, vdshwprv/IVdsAsync
ms.topic: interface
req.header: vdshwprv.h
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
 - IVdsAsync
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsAsync interface


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Manages asynchronous 
   operations. Methods that initiate asynchronous operations return a pointer to an 
   <b>IVdsAsync</b> interface, allowing the caller to optionally 
   cancel, wait for, or query the status of the asynchronous operation.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVdsAsync</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IVdsAsync</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVdsAsync</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/40940cb8-46b7-4483-9952-ab053c49dad7">Cancel</a>
</td>
<td align="left" width="63%">
Cancels the asynchronous operation.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/993228ae-4817-4d88-8544-9cd57cbe8b49">QueryStatus</a>
</td>
<td align="left" width="63%">
Returns when the asynchronous operation is in progress, or has either finished successfully or failed.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1bb30247-efb8-488f-b142-8912c351f5f2">Wait</a>
</td>
<td align="left" width="63%">
Returns when the asynchronous operation has either finished successfully or failed.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/0f809c71-a3bd-4c62-8086-9651ea1a3400">Helper Objects</a>



<a href="https://msdn.microsoft.com/372eff29-7481-45aa-ad66-73147f7a631f">IEnumVdsObject::Next</a>



<a href="https://msdn.microsoft.com/e5136e15-3ae1-4e0a-ae97-fcf16203b21d">Managing Asynchronous Operations</a>



<a href="https://msdn.microsoft.com/0bddfd62-881d-4fda-b303-ed38d434af55">VDS Interfaces</a>
 

 

