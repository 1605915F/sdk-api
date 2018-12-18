---
UID: NE:windowsstoragecom.HANDLE_OPTIONS
title: HANDLE_OPTIONS
author: windows-sdk-content
description: Defines the flags of the file handle.
old-location: winrt\handle_options.htm
tech.root: WinRT
ms.assetid: 3FB2731B-53D1-4216-9149-7D8BDE8D3F12
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HANDLE_OPTIONS, HANDLE_OPTIONS enumeration [Windows Runtime], HO_DELETE_ON_CLOSE, HO_NONE, HO_NO_BUFFERING, HO_OPEN_REQUIRING_OPLOCK, HO_OVERLAPPED, HO_RANDOM_ACCESS, HO_SEQUENTIAL_SCAN, HO_WRITE_THROUGH, windowsstoragecom/HANDLE_OPTIONS, windowsstoragecom/HO_DELETE_ON_CLOSE, windowsstoragecom/HO_NONE, windowsstoragecom/HO_NO_BUFFERING, windowsstoragecom/HO_OPEN_REQUIRING_OPLOCK, windowsstoragecom/HO_OVERLAPPED, windowsstoragecom/HO_RANDOM_ACCESS, windowsstoragecom/HO_SEQUENTIAL_SCAN, windowsstoragecom/HO_WRITE_THROUGH, winrt.handle_options
ms.topic: enum
req.header: windowsstoragecom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - HeaderDef
api_location:
 - windowsstoragecom.h
api_name:
 - HANDLE_OPTIONS
product: Windows
targetos: Windows
req.typenames: HANDLE_OPTIONS
req.redist: 
---

# HANDLE_OPTIONS enumeration


## -description


Defines the flags of the file handle.


## -enum-fields




### -field HO_NONE

None.


### -field HO_OPEN_REQUIRING_OPLOCK

This value is for internal use only.


### -field HO_DELETE_ON_CLOSE

The file is to be deleted immediately after this handle is closed.



### -field HO_SEQUENTIAL_SCAN

Access is intended to be sequential from beginning to end. The system can use this as a hint to optimize file caching.
For additional information, see <a href="https://msdn.microsoft.com/library/windows/desktop/aa363858(v=vs.85).aspx">Caching Behavior</a>.


### -field HO_RANDOM_ACCESS

Access is intended to be random. The system can use this as a hint to optimize file caching.
For more information, see  <a href="https://msdn.microsoft.com/library/windows/desktop/aa363858(v=vs.85).aspx">Caching Behavior</a>.


### -field HO_NO_BUFFERING

The file is being opened with no system caching for data reads and writes. This flag does not affect hard disk caching or memory mapped files.
There are strict requirements for successfully working with files opened with this flag. For details see  <a href="https://msdn.microsoft.com/library/windows/desktop/cc644950(v=vs.85).aspx">File Buffering</a>.


### -field HO_OVERLAPPED

The file is being opened or created for asynchronous I/O.
For information about considerations when using a file handle created with this flag, see  <a href="https://msdn.microsoft.com/library/windows/desktop/aa363858(v=vs.85).aspx">Synchronous and Asynchronous I/O Handles</a>.


### -field HO_WRITE_THROUGH

Write operations will not go through any intermediate cache, they will go directly to disk.
For additional information, see  <a href="https://msdn.microsoft.com/library/windows/desktop/aa363858(v=vs.85).aspx">Caching Behavior</a>.


