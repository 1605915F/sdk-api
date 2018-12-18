---
UID: NF:comsvcs.ISecurityProperty.GetDirectCreatorSID
title: ISecurityProperty::GetDirectCreatorSID
author: windows-sdk-content
description: In MTS 2.0, this method retrieves the security identifier of the external process that directly created the current object. Do not use this method in COM+.
old-location: cos\isecurityproperty_getdirectcreatorsid.htm
tech.root: cossdk
ms.assetid: cd06e71b-563a-45d2-91fb-f57375016dc3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDirectCreatorSID, GetDirectCreatorSID method [COM+], GetDirectCreatorSID method [COM+],ISecurityProperty interface, ISecurityProperty interface [COM+],GetDirectCreatorSID method, ISecurityProperty.GetDirectCreatorSID, ISecurityProperty::GetDirectCreatorSID, _cos_ISecurityProperty_GetDirectCreatorSID, comsvcs/ISecurityProperty::GetDirectCreatorSID, cos.isecurityproperty_getdirectcreatorsid
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
 - ISecurityProperty.GetDirectCreatorSID
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISecurityProperty::GetDirectCreatorSID


## -description


In MTS 2.0, this method retrieves the security identifier of the external process that directly created the current object. Do not use this method in COM+.


## -parameters




### -param pSID [out]

A reference to the security ID of the process that directly created the current object.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, E_UNEXPECTED, and E_FAIL, as well as the following values.

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
The security ID of the process that directly created the current object is returned in the parameter <i>pSid</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>CONTEXT_E_NOCONTEXT</b></dt>
</dl>
</td>
<td width="60%">
The current object does not have a context associated with it because either the component was not imported into an application or the object was not created with one of the COM+ CreateInstance methods.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/9395bc9a-dfe5-428a-839f-1c4ad090f636">IObjectContext</a>



<a href="https://msdn.microsoft.com/116715a5-a3e1-48aa-b155-107ea330b7ee">ISecurityProperty</a>
 

 

