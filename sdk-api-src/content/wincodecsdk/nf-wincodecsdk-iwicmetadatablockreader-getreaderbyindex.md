---
UID: NF:wincodecsdk.IWICMetadataBlockReader.GetReaderByIndex
title: IWICMetadataBlockReader::GetReaderByIndex (wincodecsdk.h)
author: windows-sdk-content
description: Retrieves an IWICMetadataReader for a specified top level metadata block.
old-location: wic\_wic_codec_iwicmetadatablockreader_getreaderbyindex.htm
tech.root: wic
ms.assetid: fb0d0951-7bb1-4bf7-9bfb-50f522929baf
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetReaderByIndex, GetReaderByIndex method [Windows Imaging Component], GetReaderByIndex method [Windows Imaging Component],IWICMetadataBlockReader interface, IWICMetadataBlockReader interface [Windows Imaging Component],GetReaderByIndex method, IWICMetadataBlockReader.GetReaderByIndex, IWICMetadataBlockReader::GetReaderByIndex, _wic_codec_iwicmetadatablockreader_getreaderbyindex, wic._wic_codec_iwicmetadatablockreader_getreaderbyindex, wincodecsdk/IWICMetadataBlockReader::GetReaderByIndex
ms.topic: method
req.header: wincodecsdk.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wincodecsdk.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Windowscodecs.lib
req.dll: Windowscodecs.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Windowscodecs.dll
api_name:
 - IWICMetadataBlockReader.GetReaderByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWICMetadataBlockReader::GetReaderByIndex


## -description


Retrieves an <a href="https://msdn.microsoft.com/0495ecf1-128a-4576-8420-0e79f1454015">IWICMetadataReader</a> for a specified top level metadata block.


## -parameters




### -param nIndex [in]

Type: <b>UINT</b>

The index of the desired top level metadata block to retrieve.


### -param ppIMetadataReader [out]

Type: <b><a href="https://msdn.microsoft.com/0495ecf1-128a-4576-8420-0e79f1454015">IWICMetadataReader</a>**</b>

When this method returns, contains a pointer to the <a href="https://msdn.microsoft.com/0495ecf1-128a-4576-8420-0e79f1454015">IWICMetadataReader</a> specified by <i>nIndex</i>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/58f03dc2-cc31-4d76-b75a-f332da1f900f">How to Write a WIC-Enabled CODEC</a>



<a href="https://msdn.microsoft.com/09614b44-ebc2-44f4-9755-9df62f1b2178">IWICMetadataBlockReader</a>



<b>Other Resources</b>



<a href="https://msdn.microsoft.com/b1e0b936-a13a-42dd-8470-957ba1d90423">Overview of Reading and Writing Image Metadata</a>



<a href="https://msdn.microsoft.com/35727810-3c4c-4c11-a4a2-3ae2cf3b8142">WIC Metadata Overview</a>



<a href="https://msdn.microsoft.com/a05b496a-bd4c-4065-8060-df0f8930cde7">Windows Imaging Component Overview</a>
 

 

