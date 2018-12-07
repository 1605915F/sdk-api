---
UID: NN:wmp.IWMPCdrom
title: IWMPCdrom
author: windows-sdk-content
description: The IWMPCdrom interface provides a way to access a CD or DVD in its drive.
old-location: wmp\iwmpcdrom.htm
tech.root: WMP
ms.assetid: 323a6841-ffbd-4bbb-ac04-1d121cf5bd06
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPCdrom, IWMPCdrom interface [Windows Media Player], IWMPCdrom interface [Windows Media Player],described, IWMPCdromInterface, wmp.iwmpcdrom, wmp/IWMPCdrom
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - wmp.h
api_name:
 - IWMPCdrom
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPCdrom interface


## -description



The <b>IWMPCdrom</b> interface provides a way to access a CD or DVD in its drive.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMPCdrom</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IWMPCdrom</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMPCdrom</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1b17c405-0887-4948-b375-c1ebcf2a72b3">eject</a>
</td>
<td align="left" width="63%">
Ejects the CD or DVD from the drive.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/0bc7766b-1e5d-4ed4-8016-aa1e8e0a7cc1">get_driveSpecifier</a>
</td>
<td align="left" width="63%">
Retrieves the CD or DVD drive letter.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c726ac41-0662-4134-b187-035f941b9df9">get_playlist</a>
</td>
<td align="left" width="63%">
Retrieves a pointer to an <b>IWMPPlaylist</b> interface representing the tracks on a CD or the root-level title entries for a DVD.

</td>
</tr>
</table> 

Retrieve a pointer to an <b>IWMPCdrom</b> interface with the following method.

<table>
<tr>
<th>Interface</th>
<th>Method</th>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/ba55ac32-149d-4f7b-a2bb-1fdb0be806cd">IWMPCdromCollection</a>
</td>
<td>
<a href="https://msdn.microsoft.com/4604e53d-914f-4888-99c7-64d0683ac2e0">item</a>
</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/04b6d6bc-a3fe-4b3f-b348-0f6b9f6e77a9">IWMPPlaylist Interface</a>



<a href="https://msdn.microsoft.com/68a0bdaf-ae1b-4ba1-817b-a31c68b9fddd">Interfaces</a>
 

 

