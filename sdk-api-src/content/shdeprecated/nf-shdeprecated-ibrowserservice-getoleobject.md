---
UID: NF:shdeprecated.IBrowserService.GetOleObject
title: IBrowserService::GetOleObject
author: windows-sdk-content
description: Deprecated. Retrieves an IOleObject for the browser.
old-location: shell\IBrowserService_GetOleObject.htm
tech.root: shell
ms.assetid: 6ac2346f-3bfb-498f-97c7-77dc431567c7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetOleObject, GetOleObject method [Windows Shell], GetOleObject method [Windows Shell],IBrowserService interface, IBrowserService interface [Windows Shell],GetOleObject method, IBrowserService.GetOleObject, IBrowserService::GetOleObject, shdeprecated/IBrowserService::GetOleObject, shell.IBrowserService_GetOleObject, zone_IBrowserService_GetOleObject
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shdeprecated.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shdeprecated.idl
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
 - Shdeprecated.h
api_name:
 - IBrowserService.GetOleObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: Internet Explorer 4.0
---

# IBrowserService::GetOleObject


## -description


Deprecated. Retrieves an <a href="https://msdn.microsoft.com/58b32c87-39b6-4d64-9174-cf798ed302c2">IOleObject</a> for the browser.


## -parameters




### -param ppobjv [out]

Type: <b><a href="https://msdn.microsoft.com/58b32c87-39b6-4d64-9174-cf798ed302c2">IOleObject</a>**</b>

The address that receives a pointer to the retrieved <a href="https://msdn.microsoft.com/58b32c87-39b6-4d64-9174-cf798ed302c2">IOleObject</a>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



