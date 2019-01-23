---
UID: NF:chstring.CHString.Right
title: CHString::Right
author: windows-sdk-content
description: Extracts the last nCount characters from a CHString string and returns a copy of the extracted substring.
old-location: wmi\chstring_right.htm
tech.root: WmiSdk
ms.assetid: eccf928f-75ac-4442-90f9-0e0578c5798f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "?Right@CHString@@QBE?AV1@H@Z, ?Right@CHString@@QEBA?AV1@H@Z, CHString interface [Windows Management Instrumentation],Right method, CHString.Right, CHString::Right, Right, Right method [Windows Management Instrumentation], Right method [Windows Management Instrumentation],CHString interface, _hmm_chstring_right, chstring/CHString::Right, wmi.chstring_right"
ms.topic: method
req.header: chstring.h
req.include-header: FwCommon.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: FrameDyn.lib
req.dll: FrameDynOS.dll; FrameDyn.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - FrameDynOS.dll
 - FrameDyn.dll
api_name:
 - CHString.Right
 - ?Right@CHString@@QBE?AV1@H@Z
 - ?Right@CHString@@QEBA?AV1@H@Z
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CHString::Right


## -description


<p class="CCE_Message">[The <a href="https://msdn.microsoft.com/e2e4378f-d842-4bca-bffc-a60e718caed3">CHString</a> class 
    is part of the WMI Provider Framework which is now considered in final state, and no further development, 
    enhancements, or updates will be available for non-security related issues affecting these libraries. The 
    <a href="https://msdn.microsoft.com/7F311E1B-5CE6-488D-9411-DE1822D95C3B">MI APIs</a> should be used for all new 
    development.]

The <b>Right</b> method extracts the last (that is, rightmost) <i>nCount</i> characters from a <a href="https://msdn.microsoft.com/e2e4378f-d842-4bca-bffc-a60e718caed3">CHString</a> string and returns a copy of the extracted substring. If <i>nCount</i> exceeds the string length, then the entire string is extracted.


## -parameters




### -param nCount

The number of characters extracted from the <a href="https://msdn.microsoft.com/e2e4378f-d842-4bca-bffc-a60e718caed3">CHString</a> string.


## -returns



Returns a <a href="https://msdn.microsoft.com/e2e4378f-d842-4bca-bffc-a60e718caed3">CHString</a> object that contains a copy of the specified range of characters.

<div class="alert"><b>Note</b>  The returned <a href="https://msdn.microsoft.com/e2e4378f-d842-4bca-bffc-a60e718caed3">CHString</a> object can be empty.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/e2e4378f-d842-4bca-bffc-a60e718caed3">CHString</a>



<a href="https://msdn.microsoft.com/52219bbb-0a88-47b3-ac6c-ba54d15e8157">CHString::Left</a>



<a href="https://msdn.microsoft.com/2036813b-f991-4ca3-95d3-8bbe858aae09">CHString::Mid</a>
 

 

