---
UID: NF:shdeprecated.IBrowserService2.OnSize
title: IBrowserService2::OnSize (shdeprecated.h)
author: windows-sdk-content
description: Deprecated. Calls the derived class from the base class on receipt of a WM_SIZE message. The derived class handles the message.
old-location: shell\IBrowserService2_OnSize.htm
tech.root: shell
ms.assetid: 082eabc4-6807-4d40-aa06-f7d230039073
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBrowserService2 interface [Windows Shell],OnSize method, IBrowserService2.OnSize, IBrowserService2::OnSize, OnSize, OnSize method [Windows Shell], OnSize method [Windows Shell],IBrowserService2 interface, shdeprecated/IBrowserService2::OnSize, shell.IBrowserService2_OnSize, zone_IBrowserService2_OnSize
ms.topic: method
req.header: shdeprecated.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - IBrowserService2.OnSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: Internet Explorer 5.0
---

# IBrowserService2::OnSize


## -description


Deprecated. Calls the derived class from the base class on receipt of a <a href="https://msdn.microsoft.com/en-us/library/ms632646(v=VS.85).aspx">WM_SIZE</a> message. The derived class handles the message.


## -parameters




### -param wParam [in]

Type: <b>WPARAM</b>

Additional information provided by the <a href="https://msdn.microsoft.com/en-us/library/ms632646(v=VS.85).aspx">WM_SIZE</a> message.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



