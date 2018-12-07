---
UID: NF:comsvcs.ICrmMonitorClerks.Description
title: ICrmMonitorClerks::Description
author: windows-sdk-content
description: Retrieves the description of the CRM Compensator for the specified index.
old-location: cos\icrmmonitorclerks_description.htm
tech.root: cossdk
ms.assetid: 3603d898-1601-419b-b3f8-3ad49f2070a0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Description, Description method [COM+], Description method [COM+],ICrmMonitorClerks interface, ICrmMonitorClerks interface [COM+],Description method, ICrmMonitorClerks.Description, ICrmMonitorClerks::Description, _dtc_ICrmMonitorClerks_Description, comsvcs/ICrmMonitorClerks::Description, cos.icrmmonitorclerks_description
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - ComSvcs.h
api_name:
 - ICrmMonitorClerks.Description
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICrmMonitorClerks::Description


## -description


Retrieves the description of the CRM Compensator for the specified index.


## -parameters




### -param Index [in]

The index of the required CRM clerk as a numeric <b>Variant</b>, or the instance CLSID as a <b>Variant</b> string.


### -param pItem [out]

The description string originally provided by <a href="https://msdn.microsoft.com/en-us/library/ms688384(v=VS.85).aspx">ICrmLogControl::RegisterCompensator</a>.


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
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A <b>NULL</b> pointer was provided as an argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One of the arguments is incorrect.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms684207(v=VS.85).aspx">ICrmMonitorClerks</a>
 

 

