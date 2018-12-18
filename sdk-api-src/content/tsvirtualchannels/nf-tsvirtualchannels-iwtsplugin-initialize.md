---
UID: NF:tsvirtualchannels.IWTSPlugin.Initialize
title: IWTSPlugin::Initialize
author: windows-sdk-content
description: Used for the first call that is made from the client to the plug-in.
old-location: termserv\iwtsplugin_initialize.htm
tech.root: TermServ
ms.assetid: 9216a069-4fd0-4e88-9cfa-050460b49906
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWTSPlugin interface [Remote Desktop Services],Initialize method, IWTSPlugin.Initialize, IWTSPlugin::Initialize, Initialize, Initialize method [Remote Desktop Services], Initialize method [Remote Desktop Services],IWTSPlugin interface, termserv.iwtsplugin_initialize, tsvirtualchannels/IWTSPlugin::Initialize
ms.topic: method
req.header: tsvirtualchannels.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: TsVirtualChannels.idl
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
 - TsVirtualChannels.h
api_name:
 - IWTSPlugin.Initialize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWTSPlugin::Initialize


## -description


Used for the first call that is made from the client to the plug-in. Any plug-in initialization should occur in this interface. Initialization occurs only once per plug-in.


## -parameters




### -param pChannelMgr [in]

Passed instance to the channel manager (<a href="https://msdn.microsoft.com/289f76b8-dbb5-4f80-98e9-f39f7946494b">IWTSVirtualChannelManager</a>) for the client.


## -returns



Returns <b>S_OK</b> if the call completes successfully. If the call fails, the plug-in will be released by the Remote Desktop Connection (RDC) client.




## -see-also




<a href="https://msdn.microsoft.com/e34caf2c-1eb6-40eb-9407-20ed4fde9cdb">IWTSPlugin</a>
 

 

