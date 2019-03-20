---
UID: NF:atscpsipparser.ISCTE_EAS.GetTableDescriptorByIndex
title: ISCTE_EAS::GetTableDescriptorByIndex (atscpsipparser.h)
author: windows-sdk-content
description: The GetTableDescriptorByIndex method returns a descriptor for the EAS table.
old-location: mstv\iscte_eas_gettabledescriptorbyindex.htm
tech.root: mstv
ms.assetid: 24e02875-32ab-4844-bec3-8044b03b9843
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetTableDescriptorByIndex, GetTableDescriptorByIndex method [Microsoft TV Technologies], GetTableDescriptorByIndex method [Microsoft TV Technologies],ISCTE_EAS interface, ISCTE_EAS interface [Microsoft TV Technologies],GetTableDescriptorByIndex method, ISCTE_EAS.GetTableDescriptorByIndex, ISCTE_EAS::GetTableDescriptorByIndex, ISCTE_EASGetTableDescriptorByIndex, atscpsipparser/ISCTE_EAS::GetTableDescriptorByIndex, mstv.iscte_eas_gettabledescriptorbyindex
ms.topic: method
req.header: atscpsipparser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: None supported
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
 - atscpsipparser.h
api_name:
 - ISCTE_EAS.GetTableDescriptorByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISCTE_EAS::GetTableDescriptorByIndex


## -description


The <b>GetTableDescriptorByIndex</b> method returns a descriptor for the EAS table.


## -parameters




### -param dwIndex [in]

The zero-based index of the descriptor to retrieve. Call the <a href="https://msdn.microsoft.com/1d6cae55-233f-49e0-8ced-9dd21b0aa32b">ISCTE_EAS::GetCountOfTableDescriptors</a> method to get the number of table descriptors.
          


### -param ppDescriptor [out]

Receives a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd694093(v=VS.85).aspx">IGenericDescriptor</a> interface. The caller must release the interface.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_OUT_OF_BOUNDS</b></dt>
</dl>
</td>
<td width="60%">
Index out of bounds.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_UNINITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/f40e89f4-6a33-44a9-933c-bf38978f1cb2">ISCTE_EAS::Initialize</a> method was not called.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/7b5620c3-f460-4118-a8a2-9b2561bd12cf">ISCTE_EAS Interface</a>
 

 

