---
UID: NF:comsvcs.ObjectContext.IsSecurityEnabled
title: ObjectContext::IsSecurityEnabled
author: windows-sdk-content
description: Indicates whether security is enabled for the current object.
old-location: cos\objectcontext_issecurityenabled.htm
tech.root: cossdk
ms.assetid: c7b3a301-9f94-40de-a3d2-5387fb4e0596
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IsSecurityEnabled, IsSecurityEnabled method [COM+], IsSecurityEnabled method [COM+],ObjectContext interface, ObjectContext interface [COM+],IsSecurityEnabled method, ObjectContext.IsSecurityEnabled, ObjectContext::IsSecurityEnabled, _cos_ObjectContext_IsSecurityEnabled, comsvcs/ObjectContext::IsSecurityEnabled, cos.objectcontext_issecurityenabled
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
 - ObjectContext.IsSecurityEnabled
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ObjectContext::IsSecurityEnabled


## -description


Indicates whether security is enabled for the current object.


## -parameters




### -param pbIsEnabled [out]

<b>TRUE</b> if security is enabled for this object; <b>FALSE</b> otherwise.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, and E_FAIL, as well as the following values.

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
An unexpected error has occurred. This can happen if one object passes its <a href="https://msdn.microsoft.com/en-us/library/ms678909(v=VS.85).aspx">ObjectContext</a> pointer to another object and the other object calls <a href="https://msdn.microsoft.com/c7b3a301-9f94-40de-a3d2-5387fb4e0596">IsSecurityEnabled</a> using this pointer. An <b>ObjectContext</b> pointer is not valid outside the context of the object that originally obtained it.

</td>
</tr>
</table>
 




## -remarks



In the COM+ environment, server and library applications can use role-based security. <b>IsSecurityEnabled</b> returns <b>TRUE</b> when an application uses role-based security, and role-based security is enabled both for the application and the specific component that called the method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms678909(v=VS.85).aspx">ObjectContext</a>
 

 

