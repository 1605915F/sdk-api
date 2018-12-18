---
UID: NF:wmsdkidl.IWMSyncReader2.SetAllocateForOutput
title: IWMSyncReader2::SetAllocateForOutput
author: windows-sdk-content
description: The SetAllocateForOutput method sets a sample allocation callback interface for allocating output samples.
old-location: wmformat\iwmsyncreader2_setallocateforoutput.htm
tech.root: wmformat
ms.assetid: 2f0c754e-f09c-472f-8f40-3fcd0fb29c48
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMSyncReader2 interface [windows Media Format],SetAllocateForOutput method, IWMSyncReader2.SetAllocateForOutput, IWMSyncReader2::SetAllocateForOutput, IWMSyncReader2SetAllocateForOutput, SetAllocateForOutput, SetAllocateForOutput method [windows Media Format], SetAllocateForOutput method [windows Media Format],IWMSyncReader2 interface, wmformat.iwmsyncreader2_setallocateforoutput, wmsdkidl/IWMSyncReader2::SetAllocateForOutput
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
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
 - IWMSyncReader2.SetAllocateForOutput
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMSyncReader2::SetAllocateForOutput


## -description



The <b>SetAllocateForOutput</b> method sets a sample allocation callback interface for allocating output samples. This method enables you to use your own buffers for reading samples. Once set, the synchronous reader will call the <a href="https://msdn.microsoft.com/en-us/library/Dd743491(v=VS.85).aspx">IWMReaderAllocatorEx::AllocateForOutputEx</a> method every time it needs a buffer to hold an output sample.




## -parameters




### -param dwOutputNum [in]

<b>DWORD</b> containing the output number.


### -param pAllocator [in]

Pointer to an <a href="https://msdn.microsoft.com/en-us/library/Dd743490(v=VS.85).aspx">IWMReaderAllocatorEx</a> interface implemented in your application.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/da66ef5b-ec92-445c-90ba-5ee89e0def36">Allocating Buffers for File Reading</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798577(v=VS.85).aspx">IWMSyncReader2 Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798578(v=VS.85).aspx">IWMSyncReader2::GetAllocateForOutput</a>
 

 

