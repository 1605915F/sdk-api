---
UID: NF:vswriter.IVssComponent.GetBackupStamp
title: IVssComponent::GetBackupStamp
author: windows-sdk-content
description: The GetBackupStamp method returns the backup stamp string stored by a writer for a given component.
old-location: base\ivsscomponent_getbackupstamp.htm
tech.root: VSS
ms.assetid: a8f272d8-4024-46bf-a0e6-77d870615fc0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetBackupStamp, GetBackupStamp method [VSS], GetBackupStamp method [VSS],IVssComponent interface, IVssComponent interface [VSS],GetBackupStamp method, IVssComponent.GetBackupStamp, IVssComponent::GetBackupStamp, _win32_ivsscomponent_getbackupstamp, base.ivsscomponent_getbackupstamp, vswriter/IVssComponent::GetBackupStamp
ms.topic: method
req.header: vswriter.h
req.include-header: Vss.h, VsWriter.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
req.lib: VssApi.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - VssApi.lib
 - VssApi.dll
api_name:
 - IVssComponent.GetBackupStamp
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVssComponent::GetBackupStamp


## -description


The 
<b>GetBackupStamp</b> method returns the backup stamp string stored by a writer for a given component.

Either a writer or a requester can call this method.


## -parameters




### -param pbstrBackupStamp [out]

The address of a caller-allocated variable that receives a string containing the backup stamp indicating the time at which the component was backed up.


## -returns



The following are the valid return codes for this method.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Successfully returned the attribute value.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
There is no time stamp associated with this component.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One of the parameter values is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The caller is out of memory or other system resources.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VSS_E_INVALID_XML_DOCUMENT</b></dt>
</dl>
</td>
<td width="60%">
The XML document is not valid. Check the event log for details. For more information, see 
<a href="https://msdn.microsoft.com/6377d937-5739-45f5-9195-5d18be4069ce">Event and Error Handling Under VSS</a>.

</td>
</tr>
</table>
 




## -remarks



If no backup time stamp has been set, 
<b>GetBackupStamp</b> returns S_FALSE.

If the call to <b>GetBackupStamp</b> is successful, the caller is responsible for freeing the string that  is returned in the <i>pbstrBackupStamp</i> parameter by calling the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function.

The string returned refers to all files in the component and any nonselectable subcomponents it has.

The backup stamp retrieved by 
<b>GetBackupStamp</b> is generally set by a writer by a call to 
<a href="https://msdn.microsoft.com/54995cc9-8988-4f26-9c60-5d809a93e4e1">IVssComponent::SetBackupStamp</a> from within the <a href="https://msdn.microsoft.com/en-us/library/Aa384664(v=VS.85).aspx">PostSnapshot</a> event handler, 
<a href="https://msdn.microsoft.com/d97d4246-882e-49c3-a214-d8d3887c1508">CVssWriter::OnPostSnapshot</a>.

Requesters merely store the backup stamps in the Backup Components Document; they do not make direct use of the backup stamp, know how to generate it, or understand its format.




## -see-also




<a href="https://msdn.microsoft.com/cc1c75bf-b281-4741-9273-f7264532860f">IVssBackupComponents::SetPreviousBackupStamp</a>



<a href="https://msdn.microsoft.com/c686a424-b0b9-4efc-8dc6-b92193de2a5d">IVssComponent</a>



<a href="https://msdn.microsoft.com/54995cc9-8988-4f26-9c60-5d809a93e4e1">IVssComponent::SetBackupStamp</a>
 

 

