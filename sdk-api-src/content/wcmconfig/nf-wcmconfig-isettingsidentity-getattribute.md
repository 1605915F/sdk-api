---
UID: NF:wcmconfig.ISettingsIdentity.GetAttribute
title: ISettingsIdentity::GetAttribute (wcmconfig.h)
author: windows-sdk-content
description: Gets an identity attribute for a namespace identity.
old-location: smi\isettingsidentity_getattribute.htm
tech.root: SMI
ms.assetid: d79bf4be-f3ed-426b-a880-b9ab8aee0092
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAttribute, GetAttribute method [SMI], GetAttribute method [SMI],ISettingsIdentity interface, ISettingsIdentity interface [SMI],GetAttribute method, ISettingsIdentity.GetAttribute, ISettingsIdentity::GetAttribute, smi.isettingsidentity_getattribute, wcmconfig/ISettingsIdentity::GetAttribute
ms.topic: method
req.header: wcmconfig.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WcmConfig.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: SMIEngine.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - SMIEngine.dll
api_name:
 - ISettingsIdentity.GetAttribute
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISettingsIdentity::GetAttribute


## -description


Gets an identity attribute for a namespace identity.


## -parameters




### -param Reserved [in]

Reserved. Must be <b>NULL</b>.


### -param Name [in]

The name of the attribute.


### -param Value [out]

The value of the attribute.


## -returns



This method returns an HRESULT value. <b>S_OK</b> indicates success. If the attribute specified by Name is not recognized, this function returns <b>WCM_E_ATTRIBUTENOTFOUND</b>.




## -see-also




<a href="https://msdn.microsoft.com/aa9d5604-5b94-47d9-9e68-d708a656a5ea">ISettingsIdentity</a>
 

 

