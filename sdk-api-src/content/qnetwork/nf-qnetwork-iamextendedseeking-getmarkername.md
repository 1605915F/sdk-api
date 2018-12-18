---
UID: NF:qnetwork.IAMExtendedSeeking.GetMarkerName
title: IAMExtendedSeeking::GetMarkerName
author: windows-sdk-content
description: The GetMarkerName method retrieves the name associated with the specified marker.
old-location: dshow\iamextendedseeking_getmarkername.htm
tech.root: DirectShow
ms.assetid: 899cc32e-3a9f-4be0-97a9-2ddd323bf9ce
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMarkerName, GetMarkerName method [DirectShow], GetMarkerName method [DirectShow],IAMExtendedSeeking interface, IAMExtendedSeeking interface [DirectShow],GetMarkerName method, IAMExtendedSeeking.GetMarkerName, IAMExtendedSeeking::GetMarkerName, IAMExtendedSeekingGetMarkerName, dshow.iamextendedseeking_getmarkername, qnetwork/IAMExtendedSeeking::GetMarkerName
ms.topic: method
req.header: qnetwork.h
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
 - COM
api_location:
 - Qnetwork.h
api_name:
 - IAMExtendedSeeking.GetMarkerName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMExtendedSeeking::GetMarkerName


## -description



The <code>GetMarkerName</code> method retrieves the name associated with the specified marker.




## -parameters




### -param MarkerNum [in]

Specifies the marker number.


### -param pbstrMarkerName [out]

Pointer to a variable that receives the marker name.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -remarks



The caller must release the returned <b>BSTR</b> by calling <b>SysFreeString</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd389331(v=VS.85).aspx">IAMExtendedSeeking Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd389334(v=VS.85).aspx">IAMExtendedSeeking::GetMarkerTime</a>
 

 

