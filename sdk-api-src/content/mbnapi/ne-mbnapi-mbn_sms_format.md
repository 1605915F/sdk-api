---
UID: NE:mbnapi.MBN_SMS_FORMAT
title: MBN_SMS_FORMAT (mbnapi.h)
author: windows-sdk-content
description: Format of SMS messages.
old-location: mbn\mbn_sms_format.htm
tech.root: mbn
ms.assetid: ece079e2-43a2-4ca9-9aa7-1b9484f0176e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MBN_SMS_FORMAT, MBN_SMS_FORMAT enumeration [Microsoft Broadband Networks], MBN_SMS_FORMAT_NONE, MBN_SMS_FORMAT_PDU, MBN_SMS_FORMAT_TEXT, mbn.mbn_sms_format, mbnapi/MBN_SMS_FORMAT, mbnapi/MBN_SMS_FORMAT_NONE, mbnapi/MBN_SMS_FORMAT_PDU, mbnapi/MBN_SMS_FORMAT_TEXT
ms.topic: enum
f1_keywords: 
 - "mbnapi/MBN_SMS_FORMAT"
req.header: mbnapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mbnapi.idl
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
 - mbnapi.h
api_name:
 - MBN_SMS_FORMAT
targetos: Windows
req.typenames: MBN_SMS_FORMAT
req.redist: 
ms.custom: 19H1
---

# MBN_SMS_FORMAT enumeration


## -description


The <b>MBN_SMS_FORMAT</b> enumerated type specifies the format of SMS messages. 


## -enum-fields




### -field MBN_SMS_FORMAT_NONE

No SMS format.


### -field MBN_SMS_FORMAT_PDU

For GSM devices, SMS, messages will be read in PDU format. 

For CDMA devices, SMS messages will be read in binary CDMA format.


### -field MBN_SMS_FORMAT_TEXT

For CDMA devices, SMS messages will be read in text format.

