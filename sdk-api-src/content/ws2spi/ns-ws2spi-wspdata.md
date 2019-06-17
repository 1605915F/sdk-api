---
UID: NS:ws2spi.WSPData
title: WSPDATA (ws2spi.h)
author: windows-sdk-content
description: The WSPDATA structure contains service provider information.
old-location: winsock\wspdata_2.htm
tech.root: WinSock
ms.assetid: 0592aa8f-5fac-4bbd-9fb8-e61d374ad0a6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPWSPDATA, LPWSPDATA, LPWSPDATA structure pointer [Winsock], WSPDATA, WSPDATA structure [Winsock], _win32_wspdata_2, winsock.wspdata_2, ws2spi/LPWSPDATA, ws2spi/WSPDATA"
ms.topic: struct
f1_keywords: ["ws2spi/WSPDATA"]
req.header: ws2spi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Ws2spi.h
api_name:
 - WSPDATA
product: Windows
targetos: Windows
req.typenames: WSPDATA, *LPWSPDATA
req.redist: 
ms.custom: 19H1
---

# WSPDATA structure


## -description


The 
<b>WSPDATA</b> structure contains service provider information.


## -struct-fields




### -field wVersion

Version of the Windows Sockets SPI specification that the Windows Sockets service provider expects the caller to use.


### -field wHighVersion

Highest version of the Windows Sockets SPI specification that this service provider can support (also encoded as above). Normally this will be the same as <b>wVersion</b>.


### -field szDescription

Null-terminated Unicode string into which the Windows Sockets provider copies a description of itself. The text (up to 256 characters in length) can contain any characters except control and formatting characters: the most likely use to which an SPI client will put this is to display it (possibly truncated) in a status message.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/ws2spi/nf-ws2spi-wspstartup">WSPStartup</a>
 

 

