---
UID: NF:credentialprovider.ICredentialProviderCredential.GetFieldState
title: ICredentialProviderCredential::GetFieldState
author: windows-sdk-content
description: Retrieves the field state. The Logon UI and Credential UI use this to gain information about a field of a credential to display this information in the user tile.
old-location: shell\ICredentialProviderCredential_GetFieldState.htm
tech.root: shell
ms.assetid: 9a709835-cf89-464d-a257-d16a1312ab44
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetFieldState, GetFieldState method [Windows Shell], GetFieldState method [Windows Shell],ICredentialProviderCredential interface, ICredentialProviderCredential interface [Windows Shell],GetFieldState method, ICredentialProviderCredential.GetFieldState, ICredentialProviderCredential::GetFieldState, _shell_ICredentialProviderCredential_GetFieldState, credentialprovider/ICredentialProviderCredential::GetFieldState, shell.ICredentialProviderCredential_GetFieldState
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: credentialprovider.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Credentialprovider.idl
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
 - Credentialprovider.h
api_name:
 - ICredentialProviderCredential.GetFieldState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICredentialProviderCredential::GetFieldState


## -description


Retrieves the field state. The Logon UI and Credential UI use this to gain information about a field of a credential to display this information in the user tile.


## -parameters




### -param dwFieldID [in]

Type: <b>DWORD</b>

The identifier for the field.


### -param pcpfs [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb762489(v=VS.85).aspx">CREDENTIAL_PROVIDER_FIELD_STATE</a>*</b>

A pointer to the credential provider field state. This indicates when the field should be displayed on the user tile.


### -param pcpfis [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb762488(v=VS.85).aspx">CREDENTIAL_PROVIDER_FIELD_INTERACTIVE_STATE</a>*</b>

A pointer to the credential provider field interactive state. This indicates when the user can interact with the field.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



