---
UID: NF:dwrite.IDWriteFontFileStream.GetFileSize
title: IDWriteFontFileStream::GetFileSize
author: windows-sdk-content
description: Obtains the total size of a file.
old-location: directwrite\IDWriteFontFileStream_GetFileSize.htm
tech.root: DirectWrite
ms.assetid: 52186ddb-ea08-4615-a3df-35ea7288270c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetFileSize, GetFileSize method [Direct Write], GetFileSize method [Direct Write],IDWriteFontFileStream interface, IDWriteFontFileStream interface [Direct Write],GetFileSize method, IDWriteFontFileStream.GetFileSize, IDWriteFontFileStream::GetFileSize, directwrite.IDWriteFontFileStream_GetFileSize, dwrite/IDWriteFontFileStream::GetFileSize
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dwrite.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dwrite.lib
req.dll: Dwrite.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dwrite.dll
api_name:
 - IDWriteFontFileStream.GetFileSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFileStream::GetFileSize


## -description


 Obtains the total size of a file.


## -parameters




### -param fileSize [out]

Type: <b>UINT64*</b>

When this method returns, contains the total size of the file.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



 Implementing <b>GetFileSize</b>() for asynchronously loaded font files may require
     downloading the complete file contents. Therefore, this method should be used only for operations that
     either require a complete font file to be loaded (for example, copying a font file) or that need to make
     decisions based on the value of the file size (for example, validation against a persisted file size).




## -see-also




<a href="https://msdn.microsoft.com/792ab9be-853f-427d-a762-2da8e81423f8">IDWriteFontFileStream</a>
 

 

