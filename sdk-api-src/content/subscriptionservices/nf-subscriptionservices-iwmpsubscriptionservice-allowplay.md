---
UID: NF:subscriptionservices.IWMPSubscriptionService.allowPlay
title: IWMPSubscriptionService::allowPlay
author: windows-sdk-content
description: Note  This section describes functionality designed for use by online stores.
old-location: wmp\iwmpsubscriptionservice_allowplay.htm
tech.root: WMP
ms.assetid: 6350bf9d-f046-494f-8052-2a6f5339b4bd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPSubscriptionService interface [Windows Media Player],allowPlay method, IWMPSubscriptionService.allowPlay, IWMPSubscriptionService::allowPlay, IWMPSubscriptionServiceallowPlay, allowPlay, allowPlay method [Windows Media Player], allowPlay method [Windows Media Player],IWMPSubscriptionService interface, subscriptionservices/IWMPSubscriptionService::allowPlay, wmp.iwmpsubscriptionservice_allowplay
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: subscriptionservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 9 Series or later.
req.target-min-winversvr: 
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
 - subscriptionservices.h
api_name:
 - IWMPSubscriptionService.allowPlay
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPSubscriptionService::allowPlay


## -description



<div class="alert"><b>Note</b>  This section describes functionality designed for use by online stores. Use of this functionality outside the context of an online store is not supported.</div>
<div> </div>
The <b>allowPlay</b> method is implemented by the online store's plug-in to manage permission for Windows Media Player to play content.




## -parameters




### -param hwnd [in]

A handle to a window in which the plug-in can display a user interface.


### -param pMedia [in]

Pointer to the media object Windows Media Player is attempting to play.


### -param pfAllowPlay [out]

Pointer to a <b>BOOL</b>. If <b>true</b>, playback is allowed.


## -returns



The method returns an <b>HRESULT</b>.




## -remarks



Your code should not perform lengthy operations synchronously when Windows Media Player calls this method. Instead, you must perform time-consuming tasks on a separate worker thread.

Windows Media Player calls <b>allowPlay</b> before opening the digital media file. This gives the online store an opportunity to disallow playback of licensed content or to initiate download of a new license if the license has expired.

Because the digital media file is not open when Windows Media Player calls <b>allowPlay</b>, calling certain methods on <i>pMedia</i> may not work. For instance, attempting to retrieve metadata using <a href="https://msdn.microsoft.com/ee964f68-d44c-4e66-908b-09070a96d96f">IWMPMedia::getItemInfo</a> could fail.

The <b>allowPlay</b> method does not circumvent DRM. If the method returns <b>TRUE</b> and the license to play has not been renewed, Windows Media Player will not play the content.

The <b>allowPlay</b> method is not called when streaming protected content for which the user does not have a license.




## -see-also




<a href="https://msdn.microsoft.com/cb9d0f20-d5ca-4db9-adcc-0a803f97f196">IWMPSubscriptionService Interface</a>
 

 

