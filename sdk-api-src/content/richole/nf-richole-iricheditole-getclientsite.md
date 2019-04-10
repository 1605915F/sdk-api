---
UID: NF:richole.IRichEditOle.GetClientSite
title: IRichEditOle::GetClientSite (richole.h)
author: windows-sdk-content
description: Retrieves an IOleClientSite interface to be used when creating a new object. All objects inserted into a rich edit control must use client site interfaces returned by this function. A client site may be used with exactly one object.
old-location: controls\IRichEditOle_GetClientSite.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\richeditcontrols\richeditcontrolreference\richeditinterfaces\iricheditole\iricheditolegetclientsite.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetClientSite, GetClientSite method [Windows Controls], GetClientSite method [Windows Controls],IRichEditOle interface, IRichEditOle interface [Windows Controls],GetClientSite method, IRichEditOle.GetClientSite, IRichEditOle::GetClientSite, _win32_IRichEditOle_GetClientSite, _win32_IRichEditOle_GetClientSite_cpp, controls.IRichEditOle_GetClientSite, controls._win32_IRichEditOle_GetClientSite, richole/IRichEditOle::GetClientSite
ms.topic: method
req.header: richole.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - IRichEditOle.GetClientSite
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRichEditOle::GetClientSite


## -description


Retrieves an <a href="https://msdn.microsoft.com/dafee149-926a-4d08-a43d-5847682db645">IOleClientSite</a> interface to be used when creating a new object. All objects inserted into a rich edit control must use client site interfaces returned by this function. A client site may be used with exactly one object.


## -parameters




### -param lplpolesite

Type: <b>LPOLECLIENTSITE*</b>

The address of the <a href="https://msdn.microsoft.com/dafee149-926a-4d08-a43d-5847682db645">IOleClientSite</a> interface. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns <b>S_OK</b> on success, or a failure code otherwise. <b>E_OUTOFMEMORY</b> is returned if memory could not be allocated for the client site.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb774306(v=VS.85).aspx">IRichEditOle</a>
 

 

