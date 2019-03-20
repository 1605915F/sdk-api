---
UID: NF:wmpservices.IWMPPlugin.UnAdviseWMPServices
title: IWMPPlugin::UnAdviseWMPServices (wmpservices.h)
author: windows-sdk-content
description: The IWMPPlugin::UnAdviseWMPServices method is used to release the pointer provided by AdviseWMPServices.
old-location: wmp\iwmpplugin_unadvisewmpservices.htm
tech.root: WMP
ms.assetid: 377a6853-94fb-4467-a893-508b56637a16
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPPlugin interface [Windows Media Player],UnAdviseWMPServices method, IWMPPlugin.UnAdviseWMPServices, IWMPPlugin::UnAdviseWMPServices, IWMPPluginUnAdviseWMPServicesDSP, UnAdviseWMPServices, UnAdviseWMPServices method [Windows Media Player], UnAdviseWMPServices method [Windows Media Player],IWMPPlugin interface, wmp.iwmpplugin_unadvisewmpservices, wmpservices/IWMPPlugin::UnAdviseWMPServices
ms.topic: method
req.header: wmpservices.h
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
 - wmpservices.h
api_name:
 - IWMPPlugin.UnAdviseWMPServices
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPPlugin::UnAdviseWMPServices


## -description



The <b>IWMPPlugin::UnAdviseWMPServices</b> method is used to release the pointer provided by <b>AdviseWMPServices</b>.




## -parameters






## -returns



The method returns an <b>HRESULT</b>.




## -remarks



Windows Media Player calls this method when the pointer provided by <b>AdviseWMPServices</b> is no longer valid. The plug-in should use this method to cease making stream state requests through the pointer.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd563582(v=VS.85).aspx">IWMPPlugin Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563599(v=VS.85).aspx">IWMPPlugin::AdviseWMPServices</a>
 

 

