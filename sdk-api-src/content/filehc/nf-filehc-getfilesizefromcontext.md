---
UID: NF:filehc.GetFileSizeFromContext
title: GetFileSizeFromContext function (filehc.h)
author: windows-sdk-content
description: Reports the file size cached with the handle.
old-location: winprog\_getfilesizefromcontext.htm
tech.root: DevNotes
ms.assetid: c44aab72-d5c8-43e0-b2ec-032904806227
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetFileSizeFromContext, GetFileSizeFromContext function [Windows API], filehc/GetFileSizeFromContext, winprog._getfilesizefromcontext
ms.topic: function
f1_keywords: 
 - "filehc/GetFileSizeFromContext"
dev_langs:
 - c++
req.header: filehc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
req.lib: Fcachdll.lib
req.dll: Fcachdll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Fcachdll.dll
api_name:
 - GetFileSizeFromContext
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetFileSizeFromContext function


## -description


Reports the file size cached with the handle.


## -parameters




### -param pContext [in]

A pointer to the <a href="Http://go.microsoft.com/fwlink/p/?linkid=85304">FIO_CONTEXT</a> structure that is associated with the file.


### -param pcbFileSizeHigh [out]

A pointer to the byte count of the file.


## -returns



Returns the size of the file in bytes.




## -see-also




<a href="Http://go.microsoft.com/fwlink/p/?linkid=85304">FIO_CONTEXT</a>
 

 

