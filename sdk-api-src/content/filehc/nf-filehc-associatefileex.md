---
UID: NF:filehc.AssociateFileEx
title: AssociateFileEx function (filehc.h)
author: windows-sdk-content
description: Associates a file with an asnychronous context.
old-location: winprog\_associatefileex.htm
tech.root: DevNotes
ms.assetid: b7efaa05-e6ac-4fb8-889f-ff6fa0755476
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AssociateFileEx, AssociateFileEx function [Windows API], filehc/AssociateFileEx, winprog._associatefileex
ms.topic: function
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
 - AssociateFileEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# AssociateFileEx function


## -description


Associates a file with an asnychronous context.


## -parameters




### -param hFile [in]

A file handle that should be in the context. It is created with the FILE_FLAG_OVERLAPPED flag set for asynchronous I/O operations. 



### -param fStoreWithDots [in]

If set to <b>TRUE</b>, this object was stored with dot stuffing.


### -param fStoredWithTerminatingDot [in]

A flag that indicates whether the terminating dot is included in an object. If this parameter is set to <b>TRUE</b>, the object is stored with a terminating dot. 

The terminating dot is used by the NNTP/SMTP protocol to identify the end of message.


## -returns



Returns a pointer to the <a href="Http://go.microsoft.com/fwlink/p/?linkid=85304">FIO_CONTEXT</a> structure that was obtained. If the function fails, it returns <b>NULL</b>.




## -see-also




<a href="Http://go.microsoft.com/fwlink/p/?linkid=85304">FIO_CONTEXT</a>
 

 

