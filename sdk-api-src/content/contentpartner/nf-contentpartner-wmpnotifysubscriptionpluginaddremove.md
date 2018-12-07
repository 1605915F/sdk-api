---
UID: NF:contentpartner.WMPNotifySubscriptionPluginAddRemove
title: WMPNotifySubscriptionPluginAddRemove function
author: windows-sdk-content
description: The WMPNotifySubscriptionPluginAddRemove function notifies Windows Media Player that a COM object has been installed or uninstalled.
old-location: wmp\wmpnotifysubscriptionpluginaddremove.htm
tech.root: WMP
ms.assetid: 5217142d-fe1a-4d9f-a4e4-5d9e103ee573
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WMPNotifyPluginAddRemove_Subscriptions, WMPNotifySubscriptionPluginAddRemove, WMPNotifySubscriptionPluginAddRemove function [Windows Media Player], contentpartner/WMPNotifySubscriptionPluginAddRemove, wmp.wmpnotifysubscriptionpluginaddremove
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: contentpartner.h
req.include-header: Subscriptionservices.h
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 10 or later.
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
 - HeaderDef
api_location:
 - contentpartner.h
api_name:
 - WMPNotifySubscriptionPluginAddRemove
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WMPNotifySubscriptionPluginAddRemove function


## -description


The <b>WMPNotifySubscriptionPluginAddRemove</b> function notifies Windows Media Player that a COM object has been installed or uninstalled.
<div class="alert"><b>Note</b>  This section describes functionality designed for use by online stores. Use of this functionality outside the context of an online store is not supported.</div><div> </div>

## -parameters






## -returns



The return value indicates whether the function call succeeded.




## -remarks



This function is typically called by a plug-in in its <a href="https://msdn.microsoft.com/4442206b-b2ad-47d7-8add-18002c44c5a2">DllRegisterServer</a> and <a href="https://msdn.microsoft.com/b71137a7-284e-4521-a3b2-9dad9c9d3c54">DllUnregisterServer</a> methods. It alerts Windows Media Player to enumerate registered online store objects.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd564244(v=VS.85).aspx">Reference for Type 2 Online Stores</a>
 

 

