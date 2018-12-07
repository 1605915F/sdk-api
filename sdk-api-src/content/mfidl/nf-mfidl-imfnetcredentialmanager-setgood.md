---
UID: NF:mfidl.IMFNetCredentialManager.SetGood
title: IMFNetCredentialManager::SetGood
author: windows-sdk-content
description: Specifies whether the user's credentials succeeded in the authentication challenge. The network source calls this method to informs the application whether the user's credentials were authenticated.
old-location: mf\imfnetcredentialmanager_setgood.htm
tech.root: medfound
ms.assetid: f58e30ba-3e9b-41b5-9c13-0f9dac541033
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMFNetCredentialManager interface [Media Foundation],SetGood method, IMFNetCredentialManager.SetGood, IMFNetCredentialManager::SetGood, SetGood, SetGood method [Media Foundation], SetGood method [Media Foundation],IMFNetCredentialManager interface, f58e30ba-3e9b-41b5-9c13-0f9dac541033, mf.imfnetcredentialmanager_setgood, mfidl/IMFNetCredentialManager::SetGood
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfuuid.lib
 - mfuuid.dll
api_name:
 - IMFNetCredentialManager.SetGood
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFNetCredentialManager::SetGood


## -description



Specifies whether the user's credentials succeeded in the authentication challenge. The network source calls this method to informs the application whether the user's credentials were authenticated.




## -parameters




### -param pCred [in]

Pointer to the <a href="https://msdn.microsoft.com/d202e7bc-9ce0-4861-8552-5a4d599b1661">IMFNetCredential</a> interface.


### -param fGood [in]

Boolean value. The value is <b>TRUE</b> if the credentials succeeded in the authentication challenge. Otherwise, the value is <b>FALSE</b>.


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
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/002d8608-4ef9-40fd-8dcc-fe6ade34478e">IMFNetCredentialManager</a>
 

 

