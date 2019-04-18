---
UID: NF:casetup.ICertSrvSetup.Install
title: ICertSrvSetup::Install (casetup.h)
author: windows-sdk-content
description: Installs a role as configured in the CCertSrvSetup object.
old-location: security\icertsrvsetup_install.htm
tech.root: SecCrypto
ms.assetid: e07b1cdd-ccb6-4398-862b-521ac1d39f66
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICertSrvSetup interface [Security],Install method, ICertSrvSetup.Install, ICertSrvSetup::Install, Install, Install method [Security], Install method [Security],ICertSrvSetup interface, casetup/ICertSrvSetup::Install, security.icertsrvsetup_install
ms.topic: method
req.header: casetup.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Casetup.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Certocm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certocm.dll
api_name:
 - ICertSrvSetup.Install
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ICertSrvSetup::Install


## -description


The <b>Install</b> method installs a role as configured in the <b>CCertSrvSetup</b> object.


## -parameters






## -remarks



The <a href="https://msdn.microsoft.com/dff7e2e2-291a-4ea9-858a-8d98d96f79ac">InitializeDefaults</a> method must be called before calling this or any other method on a <b>CCertSrvSetup</b> object.

Unless the key already exists, the <b>Install</b> method creates a key for the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certification authority</a> (CA) certificate. If the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">cryptographic service provider</a> (CSP) requires interaction, it prompts the user. 




## -see-also




<a href="https://msdn.microsoft.com/6792a0d6-d304-481d-a97b-5fb7033c7eae">ICertSrvSetup</a>
 

 

