---
UID: NF:mfidl.MFCreateMFByteStreamOnStreamEx
title: MFCreateMFByteStreamOnStreamEx function
author: windows-sdk-content
description: Creates a Microsoft Media Foundation byte stream that wraps an IRandomAccessStream object.
old-location: mf\mfcreatemfbytestreamonstreamex.htm
tech.root: medfound
ms.assetid: C16C2A5D-7373-4EA9-A02C-3AF97EA47D34
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MFCreateMFByteStreamOnStreamEx, MFCreateMFByteStreamOnStreamEx function [Media Foundation], mf.mfcreatemfbytestreamonstreamex, mf.mfcreatemfbytestreamonwinrtstream, mfidl/MFCreateMFByteStreamOnStreamEx
ms.topic: function
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfplat.lib
req.dll: Mfplat.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - mfplat.dll
api_name:
 - MFCreateMFByteStreamOnStreamEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MFCreateMFByteStreamOnStreamEx function


## -description


Creates a Microsoft Media Foundation byte stream that wraps an <a href="https://msdn.microsoft.com/en-us/library/Hh438400(v=VS.85).aspx">IRandomAccessStream</a> object.


## -parameters




### -param punkStream [in]

A pointer to the <a href="https://msdn.microsoft.com/en-us/library/Hh438400(v=VS.85).aspx">IRandomAccessStream</a> interface.


### -param ppByteStream [out]

Receives a pointer to the <a href="https://msdn.microsoft.com/690035b7-2855-4714-938f-f8250ec70d24">IMFByteStream</a> interface. The caller must release the interface.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/3018ffa7-e709-45b0-8b2b-7640d5633378">Media Foundation Functions</a>
 

 

