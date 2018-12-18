---
UID: NF:richole.IRichEditOleCallback.DeleteObject
title: IRichEditOleCallback::DeleteObject
author: windows-sdk-content
description: Sends notification that an object is about to be deleted from a rich edit control. The object is not necessarily being released when this member is called.
old-location: controls\IRichEditOleCallback_DeleteObject.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\richeditcontrols\richeditcontrolreference\richeditinterfaces\iricheditolecallback\iricheditolecallbackdeleteobject.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DeleteObject, DeleteObject method [Windows Controls], DeleteObject method [Windows Controls],IRichEditOleCallback interface, IRichEditOleCallback interface [Windows Controls],DeleteObject method, IRichEditOleCallback.DeleteObject, IRichEditOleCallback::DeleteObject, _win32_IRichEditOleCallback_DeleteObject, _win32_IRichEditOleCallback_DeleteObject_cpp, controls.IRichEditOleCallback_DeleteObject, controls._win32_IRichEditOleCallback_DeleteObject, richole/IRichEditOleCallback::DeleteObject
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
 - IRichEditOleCallback.DeleteObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRichEditOleCallback::DeleteObject


## -description


Sends notification that an object is about to be deleted from a rich edit control. The object is not necessarily being released when this member is called.


## -parameters




### -param lpoleobj

Type: <b>LPOLEOBJECT</b>

The object that is being deleted. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns <b>S_OK</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb774308(v=VS.85).aspx">IRichEditOleCallback</a>
 

 

