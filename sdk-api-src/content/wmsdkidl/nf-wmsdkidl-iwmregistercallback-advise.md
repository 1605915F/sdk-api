---
UID: NF:wmsdkidl.IWMRegisterCallback.Advise
title: IWMRegisterCallback::Advise (wmsdkidl.h)
author: windows-sdk-content
description: The Advise method registers the application to receive status messages from the sink object.
old-location: wmformat\iwmregistercallback_advise.htm
tech.root: wmformat
ms.assetid: 69d12e5c-23fd-4d4b-959e-fe7979bf3fdb
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Advise, Advise method [windows Media Format], Advise method [windows Media Format],IWMRegisterCallback interface, IWMRegisterCallback interface [windows Media Format],Advise method, IWMRegisterCallback.Advise, IWMRegisterCallback::Advise, IWMRegisterCallbackAdvise, wmformat.iwmregistercallback_advise, wmsdkidl/IWMRegisterCallback::Advise
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 7 SDK, or later versions of the SDK
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
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmvcore.lib
 - Wmvcore.dll
 - WMStubDRM.lib
 - WMStubDRM.dll
api_name:
 - IWMRegisterCallback.Advise
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMRegisterCallback::Advise


## -description



The <b>Advise</b> method registers the application to receive status messages from the sink object.




## -parameters




### -param pCallback [in]

Pointer to the application's <a href="https://msdn.microsoft.com/en-us/library/Dd798544(v=VS.85).aspx">IWMStatusCallback</a> interface. The application must implement this interface.


### -param pvContext [in]

Generic pointer, for use by the application. This is passed to the application in calls to <b>OnStatus</b>.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -remarks



The sink object sends status messages to the application by calling the application's <a href="https://msdn.microsoft.com/en-us/library/Dd798545(v=VS.85).aspx">IWMStatusCallback::OnStatus</a> method.

When the application has finished using the sink object, use the <b>Unadvise</b> method to break the connection with the sink object.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd743613(v=VS.85).aspx">IWMRegisterCallback Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd743618(v=VS.85).aspx">IWMRegisterCallback::Unadvise</a>
 

 

