---
UID: NF:callobj.ICallFrame.GetInfo
title: ICallFrame::GetInfo
author: windows-sdk-content
description: Retrieves information about the call frame.
old-location: com\icallframe_getinfo.htm
tech.root: com
ms.assetid: 807b4542-c18d-48e4-8493-c40a85e5e1de
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetInfo, GetInfo method [COM], GetInfo method [COM],ICallFrame interface, ICallFrame interface [COM],GetInfo method, ICallFrame.GetInfo, ICallFrame::GetInfo, _com_icallframe_getinfo, callobj/ICallFrame::GetInfo, com.icallframe_getinfo
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: callobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Callobj.idl
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
 - Callobj.h
api_name:
 - ICallFrame.GetInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICallFrame::GetInfo


## -description


Retrieves information about the call frame.


## -parameters




### -param pInfo [out]

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms680725(v=VS.85).aspx">CALLFRAMEINFO</a> structure.


## -returns



This method can return the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
An unexpected error has occurred.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms680725(v=VS.85).aspx">CALLFRAMEINFO</a>



<a href="https://msdn.microsoft.com/en-us/library/ms683709(v=VS.85).aspx">ICallFrame</a>
 

 

