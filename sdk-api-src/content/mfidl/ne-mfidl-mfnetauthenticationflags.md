---
UID: NE:mfidl._MFNetAuthenticationFlags
title: MFNetAuthenticationFlags (mfidl.h)
author: windows-sdk-content
description: Specifies how the user's credentials will be used.
old-location: mf\mfnetauthenticationflags.htm
tech.root: medfound
ms.assetid: 4a2f5537-b78c-49a6-9b66-d3ca34c3fc67
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 4a2f5537-b78c-49a6-9b66-d3ca34c3fc67, MFNET_AUTHENTICATION_CLEAR_TEXT, MFNET_AUTHENTICATION_LOGGED_ON_USER, MFNET_AUTHENTICATION_PROXY, MFNetAuthenticationFlags, MFNetAuthenticationFlags enumeration [Media Foundation], mf.mfnetauthenticationflags, mfidl/MFNET_AUTHENTICATION_CLEAR_TEXT, mfidl/MFNET_AUTHENTICATION_LOGGED_ON_USER, mfidl/MFNET_AUTHENTICATION_PROXY, mfidl/MFNetAuthenticationFlags
ms.topic: enum
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - mfidl.h
api_name:
 - MFNetAuthenticationFlags
product: Windows
targetos: Windows
req.typenames: MFNetAuthenticationFlags
req.redist: 
---

# MFNetAuthenticationFlags enumeration


## -description



Specifies how the user's credentials will be used.




## -enum-fields




### -field MFNET_AUTHENTICATION_PROXY

The credentials will be used to authenticate with a proxy.


### -field MFNET_AUTHENTICATION_CLEAR_TEXT

The credentials will be sent over the network unencrypted.


### -field MFNET_AUTHENTICATION_LOGGED_ON_USER

The credentials must be from a user who is currently logged on.


## -see-also




<a href="https://msdn.microsoft.com/7e095445-354a-4fbb-b354-bf87eb77552f">IMFNetCredentialCache::GetCredential</a>



<a href="https://msdn.microsoft.com/f26a730f-18c4-4247-acaf-af1dfad19086">Media Foundation Enumerations</a>



<a href="https://msdn.microsoft.com/bffc33ec-0fb0-4bbe-9bac-583b9d4e1153">Network Source Authentication</a>
 

 

