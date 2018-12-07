---
UID: NF:upnp.IUPnPDevice.IconURL
title: IUPnPDevice::IconURL
author: windows-sdk-content
description: The IconURL method returns a URL from which an icon of the specified format can be loaded.
old-location: upnp\iupnpdevice_iconurl.htm
tech.root: upnp
ms.assetid: 17b3d4f1-a51a-42f9-8fc0-4156d4975889
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUPnPDevice interface [UPnP APIs],IconURL method, IUPnPDevice.IconURL, IUPnPDevice::IconURL, IconURL, IconURL method [UPnP APIs], IconURL method [UPnP APIs],IUPnPDevice interface, _upnp_iupnpdevice_iconurl, upnp.iupnpdevice_iconurl, upnp/IUPnPDevice::IconURL
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: upnp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
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
req.dll: Upnp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Upnp.dll
api_name:
 - IUPnPDevice.IconURL
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUPnPDevice::IconURL


## -description


The 
<b>IconURL</b> method returns a URL from which an icon of the specified format can be loaded.


## -parameters




### -param bstrEncodingFormat [in]

Specifies the MIME type of the encoding format that is requested for the icon.


### -param lSizeX [in]

Specifies the width of the icon, in pixels. Standard values are 16, 32, or 48.


### -param lSizeY [in]

Specifies the height of the icon, in pixels. Standard values are 16, 32, or 48 pixels.


### -param lBitDepth [in]

Specifies the bit depth of the icon. Standard values are 8, 16, or 24.


### -param pbstrIconURL [out]

Receives a reference to a string that contains the URL from which the icon is to be loaded. Release this string with <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> when it is no longer required.


## -returns



If the method succeeds, the return value is S_OK. Otherwise, the method returns one of the COM error codes defined in WinError.h.




## -remarks



An application can specify any values for <i>lSizeX</i>, <i>lSizeY</i>, and <i>lBitDepth</i>. However, there is no guarantee that an icon exists with those specifications.

If a matching icon does not exist, the URL for the icon that most closely matches the size and bit depth specified is returned.




## -see-also




<a href="https://msdn.microsoft.com/566cc606-3dfb-4052-93b0-3c922bf30f84">IUPnPDevice</a>
 

 

