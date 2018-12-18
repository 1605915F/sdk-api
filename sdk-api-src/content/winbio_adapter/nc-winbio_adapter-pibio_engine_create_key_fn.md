---
UID: NC:winbio_adapter.PIBIO_ENGINE_CREATE_KEY_FN
title: PIBIO_ENGINE_CREATE_KEY_FN
author: windows-sdk-content
description: Called by the Windows Biometric Framework to push an HMAC key to the sensor. The returned key identifier will be passed back to the biometric unit when the framework calls EngineAdapterIdentifyFeatureSetSecure.
old-location: secbiomet\engineadaptercreatekey.htm
tech.root: SecBioMet
ms.assetid: 3EB42081-6949-46F8-B235-377234A90C39
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EngineAdapterCreateKey, EngineAdapterCreateKey callback function [Windows Biometric Framework API], PIBIO_ENGINE_CREATE_KEY_FN, PIBIO_ENGINE_CREATE_KEY_FN callback, secbiomet.engineadaptercreatekey, winbio_adapter/EngineAdapterCreateKey
ms.topic: callback
req.header: winbio_adapter.h
req.include-header: Winbio_adapter.h
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - UserDefined
api_location:
 - Winbio_adapter.h
api_name:
 - EngineAdapterCreateKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PIBIO_ENGINE_CREATE_KEY_FN callback function


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Called by the Windows Biometric Framework to push an HMAC key to the sensor. The returned key identifier will be passed back to the biometric unit when the framework calls <a href="https://msdn.microsoft.com/56BD9A75-2779-4D21-A083-75736DE6880E">EngineAdapterIdentifyFeatureSetSecure</a>. 


## -parameters




### -param Pipeline

Pointer to a <a href="https://msdn.microsoft.com/b5fc2b14-b0b6-4327-a42a-ecae41c3e12a">WINBIO_PIPELINE</a> structure associated with the biometric unit performing the operation.


### -param *Key

Pointer to a buffer that contains the HMAC key.


### -param KeySize

Size, in bytes, of the buffer specified by the <b>Key</b>  parameter.


### -param KeyIdentifier

Pointer to a buffer that receives a key identifier. The format of the buffer is vendor-defined.


### -param KeyIdentifierSize

Size, in bytes, of the buffer specified by the <b>KeyIdentifier</b>  parameter.


### -param ResultSize

Pointer to a variable that receives the size, in bytes, of the data written to the buffer specified by the <b>KeyIdentifier</b>  parameter.


## -returns



If the <b>KeyIdentifier</b> buffer is too small, <b>WINBIO_E_KEY_IDENTIFIER_BUFFER_TOO_SMALL</b> must be returned, and the required size must be written to <i>ResultSize</i>. The framework will call the API again with a larger buffer.
If the sensor cannot create the key, <b>WINBIO_E_KEY_CREATION_FAILED</b> must be returned.





## -remarks



Only a single key will be in use at any time. If <b>EngineAdapterCreateKey</b> is called when the engine has knowledge of a preexisting key, the preexisting key must be overwritten with the new one.



