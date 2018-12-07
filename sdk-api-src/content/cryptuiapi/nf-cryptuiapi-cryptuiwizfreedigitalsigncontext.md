---
UID: NF:cryptuiapi.CryptUIWizFreeDigitalSignContext
title: CryptUIWizFreeDigitalSignContext function
author: windows-sdk-content
description: Frees the CRYPTUI_WIZ_DIGITAL_SIGN_CONTEXT structure allocated by the CryptUIWizDigitalSign function.
old-location: security\cryptuiwizfreedigitalsigncontext.htm
tech.root: seccrypto
ms.assetid: 039615ee-0485-4698-944f-23359253767a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CryptUIWizFreeDigitalSignContext, CryptUIWizFreeDigitalSignContext function [Security], cryptuiapi/CryptUIWizFreeDigitalSignContext, security.cryptuiwizfreedigitalsigncontext
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cryptuiapi.h
req.include-header: 
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
req.lib: Cryptui.lib
req.dll: Cryptui.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Cryptui.dll
api_name:
 - CryptUIWizFreeDigitalSignContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CryptUIWizFreeDigitalSignContext function


## -description


The <b>CryptUIWizFreeDigitalSignContext</b> function frees the <a href="https://msdn.microsoft.com/en-us/library/Aa380668(v=VS.85).aspx">CRYPTUI_WIZ_DIGITAL_SIGN_CONTEXT</a> structure allocated by the <a href="https://msdn.microsoft.com/en-us/library/Aa380292(v=VS.85).aspx">CryptUIWizDigitalSign</a> function.


## -parameters




### -param pSignContext [in]

A pointer to the   <a href="https://msdn.microsoft.com/en-us/library/Aa380668(v=VS.85).aspx">CRYPTUI_WIZ_DIGITAL_SIGN_CONTEXT</a> structure to be freed.


## -returns



If the function succeeds, the function returns nonzero.

If the function fails, it returns zero.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa380668(v=VS.85).aspx">CRYPTUI_WIZ_DIGITAL_SIGN_CONTEXT</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa380292(v=VS.85).aspx">CryptUIWizDigitalSign</a>
 

 

