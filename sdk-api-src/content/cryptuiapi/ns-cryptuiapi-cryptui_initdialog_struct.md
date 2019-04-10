---
UID: NS:cryptuiapi.tagCRYPTUI_INITDIALOG_STRUCT
title: CRYPTUI_INITDIALOG_STRUCT (cryptuiapi.h)
author: windows-sdk-content
description: Supports the CRYPTUI_VIEWCERTIFICATE_STRUCT structure.
old-location: security\cryptui_initdialog_struct.htm
tech.root: SecCrypto
ms.assetid: c6335c02-3b3e-45e2-bb58-b7213aea500b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PCRYPTUI_INITDIALOG_STRUCT, CRYPTUI_INITDIALOG_STRUCT, CRYPTUI_INITDIALOG_STRUCT structure [Security], PCRYPTUI_INITDIALOG_STRUCT, PCRYPTUI_INITDIALOG_STRUCT structure pointer [Security], cryptuiapi/CRYPTUI_INITDIALOG_STRUCT, cryptuiapi/PCRYPTUI_INITDIALOG_STRUCT, security.cryptui_initdialog_struct"
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Cryptuiapi.h
api_name:
 - CRYPTUI_INITDIALOG_STRUCT
product: Windows
targetos: Windows
req.typenames: CRYPTUI_INITDIALOG_STRUCT, *PCRYPTUI_INITDIALOG_STRUCT
req.redist: 
---

# CRYPTUI_INITDIALOG_STRUCT structure


## -description


The <b>CRYPTUI_INITDIALOG_STRUCT</b> structure supports the <a href="https://msdn.microsoft.com/en-us/library/Aa380645(v=VS.85).aspx">CRYPTUI_VIEWCERTIFICATE_STRUCT</a> structure. It  is passed as the <i>lParam</i> in the <a href="https://msdn.microsoft.com/en-us/library/ms645428(v=VS.85).aspx">WM_INITDIALOG</a> call to each
property sheet that is in the <b>rgPropSheetPages</b> array of the <a href="https://msdn.microsoft.com/en-us/library/Aa380645(v=VS.85).aspx">CRYPTUI_VIEWCERTIFICATE_STRUCT</a> structure. The <b>CRYPTUI_VIEWCERTIFICATE_STRUCT</b> structure is used in the <a href="https://msdn.microsoft.com/5107ff22-78c4-4005-80af-ff45781da6c7">CryptUIDlgViewCertificate</a> function.


## -struct-fields




### -field lParam

The <b>lParam</b> in the <a href="https://msdn.microsoft.com/en-us/library/Bb774548(v=VS.85).aspx">PROPSHEETPAGE</a> structure.


### -field pCertContext

A pointer to the <a href="https://msdn.microsoft.com/f0a3200e-6541-423d-a4a3-595a31026eea">CERT_CONTEXT</a> structure for the certificate that <a href="https://msdn.microsoft.com/5107ff22-78c4-4005-80af-ff45781da6c7">CryptUIDlgViewCertificate</a> is displaying.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa380645(v=VS.85).aspx">CRYPTUI_VIEWCERTIFICATE_STRUCT</a>



<a href="https://msdn.microsoft.com/5107ff22-78c4-4005-80af-ff45781da6c7">CryptUIDlgViewCertificate</a>
 

 

