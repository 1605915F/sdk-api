---
UID: NF:iads.IADsFileServiceOperations.Resources
title: IADsFileServiceOperations::Resources
author: windows-sdk-content
description: The IADsFileServiceOperations::Resources method gets a pointer to a pointer to the IADsCollection interface on a collection of the resource objects representing the current open resources on this file service.
old-location: adsi\iadsfileserviceoperations_resources.htm
tech.root: adsi
ms.assetid: 5b7f2240-ca92-4e8e-b3ec-8eab36c3166f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IADsFileServiceOperations interface [ADSI],Resources method, IADsFileServiceOperations.Resources, IADsFileServiceOperations::Resources, Resources, Resources method [ADSI], Resources method [ADSI],IADsFileServiceOperations interface, _ds_iadsfileserviceoperations_resources, adsi.iadsfileserviceoperations__resources, adsi.iadsfileserviceoperations_resources, iads/IADsFileServiceOperations::Resources
ms.topic: method
req.header: iads.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
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
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Activeds.dll
api_name:
 - IADsFileServiceOperations.Resources
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsFileServiceOperations::Resources


## -description


The <b>IADsFileServiceOperations::Resources</b> method gets a pointer to a pointer to the <a href="https://msdn.microsoft.com/4552552b-c008-439a-95bf-eaf9ffd28b5f">IADsCollection</a> interface on a collection of the resource objects representing the current open resources on this file service.


## -parameters




### -param ppResources [out]

Pointer to a  pointer to the <a href="https://msdn.microsoft.com/4552552b-c008-439a-95bf-eaf9ffd28b5f">IADsCollection</a> interface that can then be used to enumerate objects implementing the <a href="https://msdn.microsoft.com/217749a4-55dc-457f-8582-1513ff3b0666">IADsResource</a> interface and representing the current open resources for this file service.


## -returns



This method supports the standard return values including S_OK. For more information and other return values, see  <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>.




## -remarks



Traditional directory services supply data only about directory service elements  represented in the underlying data store. Data about resources for file services may not be available from the underlying directory store.


#### Examples

The following code example shows how to enumerate open resources managed by a file service.

<div class="code"><span codelanguage="VisualBasic"><table>
<tr>
<th>VB</th>
</tr>
<tr>
<td>
<pre>Dim fso As IADsFileServiceOperations
On Error GoTo Cleanup

' Bind to a file service operation on "myComputer" 
' in the local domain.
Set fso = GetObject("WinNT://myComputer/LanmanServer")

' Enumerate resources.
For Each resource In fso.Resources
    MsgBox "Resource path: " & resource.Path
Next resource

Cleanup:
    If (Err.Number<>0) Then
        MsgBox("An error has occurred. " & Err.Number)
    End If
    Set fso = Nothing
</pre>
</td>
</tr>
</table></span></div>


For a code example using the <b>IADsFileServiceOperations::Resources</b> method, see the code example given in  <a href="https://msdn.microsoft.com/217749a4-55dc-457f-8582-1513ff3b0666">IADsResource</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/328eedfe-7fdc-4e90-8bac-ab30944b8fbf">IADsFileService</a>



<a href="https://msdn.microsoft.com/91335658-8efb-4945-9862-f72e78d749d6">IADsFileServiceOperations</a>



<a href="https://msdn.microsoft.com/217749a4-55dc-457f-8582-1513ff3b0666">IADsResource</a>
 

 

