---
UID: NF:qnetwork.IDShowPlugin.get_UserAgent
title: IDShowPlugin::get_UserAgent
author: windows-sdk-content
description: The get_UserAgent method retrieves the User-Agent field from the HTTP header.
old-location: dshow\idshowplugin_get_useragent.htm
tech.root: DirectShow
ms.assetid: 0bbd3cd2-75d8-4c48-837d-4cb045cad35b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDShowPlugin interface [DirectShow],get_UserAgent method, IDShowPlugin.get_UserAgent, IDShowPlugin::get_UserAgent, IDShowPluginget_UserAgent, dshow.idshowplugin_get_useragent, get_UserAgent, get_UserAgent method [DirectShow], get_UserAgent method [DirectShow],IDShowPlugin interface, qnetwork/IDShowPlugin::get_UserAgent
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: qnetwork.h
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
 - COM
api_location:
 - Qnetwork.h
api_name:
 - IDShowPlugin.get_UserAgent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDShowPlugin::get_UserAgent


## -description



The <code>get_UserAgent</code> method retrieves the User-Agent field from the HTTP header.




## -parameters




### -param pUserAgent

Pointer to a variable that receives the User-Agent string.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -remarks



The caller must release the returned <b>BSTR</b>, by calling <b>SysFreeString</b>.




## -see-also




<a href="https://msdn.microsoft.com/b5b73489-4d2d-4afa-a4df-7b84711f2556">IDShowPlugin Interface</a>
 

 

