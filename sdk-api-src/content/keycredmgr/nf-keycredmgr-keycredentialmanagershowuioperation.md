---
UID: NF:keycredmgr.KeyCredentialManagerShowUIOperation
title: KeyCredentialManagerShowUIOperation function (keycredmgr.h)
author: windows-sdk-content
description: API to perform the requested WHFB operation.
old-location: security\keycredentialmanagershowuioperation.htm
tech.root: SecAuthN
ms.assetid: 94AB2BA7-810C-4AC4-A719-FD9684C21BA0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: KeyCredentialManagerShowUIOperation, KeyCredentialManagerShowUIOperation function [Security], keycredmgr/KeyCredentialManagerShowUIOperation, security.keycredentialmanagershowuioperation
ms.topic: function
req.header: keycredmgr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Keycredmgr.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - keycredmgr.lib
 - keycredmgr.dll
api_name:
 - KeyCredentialManagerShowUIOperation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# KeyCredentialManagerShowUIOperation function


## -description


API to perform the requested WHFB operation.


## -parameters




### -param hWndOwner [in]

Window handle of the calling app.


### -param keyCredentialManagerOperationType [in]

The intended operation from the <a href="https://msdn.microsoft.com/en-us/library/Mt830291(v=VS.85).aspx">KeyCredentialManagerOperationType</a>.


## -returns



Returns an HRESULT



