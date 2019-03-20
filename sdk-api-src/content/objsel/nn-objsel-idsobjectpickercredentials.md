---
UID: NN:objsel.IDsObjectPickerCredentials
title: IDsObjectPickerCredentials (objsel.h)
author: windows-sdk-content
description: The IDsObjectPickerCredentials interface allows you to override credentials for the IDsObjectPicker object implementing this interface.
old-location: ad\idsobjectpickercredentials.htm
tech.root: ad
ms.assetid: 336e7e68-0903-42f7-9810-53ccceed32de
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDsObjectPickerCredentials, IDsObjectPickerCredentials object [Active Directory], IDsObjectPickerCredentials object [Active Directory],described, ad.idsobjectpickercredentials, objsel/IDsObjectPickerCredentials
ms.topic: interface
req.header: objsel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008
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
req.dll: Objsel.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Objsel.dll
api_name:
 - IDsObjectPickerCredentials
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDsObjectPickerCredentials interface


## -description


The <b>IDsObjectPickerCredentials</b> interface 
    allows you to override credentials for the <a href="https://msdn.microsoft.com/f2f9da7d-7a09-4b49-a750-078a4573e213">IDsObjectPicker</a> 
    object implementing this interface.

To obtain an instance of this interface, call 
    <a href="https://msdn.microsoft.com/en-us/library/ms682521(v=VS.85).aspx">QueryInterface</a> with the 
    <b>IID_IDsObjectPickerCredentials</b> interface identifier as shown below.


## -members

The <b>IDsObjectPickerCredentials</b> object has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/fb1c366d-10df-4e4f-a381-3f085bd136e2">SetCredentials</a>
</td>
<td align="left" width="63%">
Sets credentials to be used by the Object Picker.

</td>
</tr>
</table>Sets credentials to be used by the Object Picker.

 

