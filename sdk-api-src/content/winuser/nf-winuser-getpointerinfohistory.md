---
UID: NF:winuser.GetPointerInfoHistory
title: GetPointerInfoHistory function
author: windows-sdk-content
description: Gets the information associated with the individual inputs, if any, that were coalesced into the current message for the specified pointer.
old-location: inputmsg\getpointerinfohistory.htm
tech.root: InputMsg
ms.assetid: 92173197-45e8-4ee7-8959-2f14f90c2d21
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPointerInfoHistory, GetPointerInfoHistory function [Input Messages and Notifications], inputmsg.getpointerinfohistory, winuser/GetPointerInfoHistory
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
 - API-MS-Win-NTUser-IE-WMPointer-l1-1-0.dll
 - ie_shims.dll
 - API-MS-Win-RTCore-NTUser-WMPointer-l1-1-0.dll
 - MinUser.dll
 - API-MS-Win-RTCore-NTUser-WMPointer-l1-1-1.dll
 - API-Ms-Win-RTCore-NTUser-WMPointer-L1-1-2.dll
 - API-MS-Win-RTCore-NTUser-WMPointer-L1-1-3.dll
api_name:
 - GetPointerInfoHistory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetPointerInfoHistory function


## -description


Gets the information associated with the individual inputs, if any, that were coalesced into the current message for the specified pointer. The most recent input is included in the returned history and is the same as the most recent input returned by the <a href="https://msdn.microsoft.com/75faea24-91cd-448b-b67a-19fe530f1800">GetPointerInfo</a> function.


## -parameters




### -param pointerId [in]

An identifier of the pointer for which to retrieve information.


### -param entriesCount [in, out]

A pointer to a variable that specifies the count of structures in the buffer to which pointerInfo points. If <b>GetPointerInfoHistory</b> succceeds, <i>entriesCount</i>  is updated with the total count of structures available. The total count of structures available is the same as the <b>historyCount</b> field of the <a href="https://msdn.microsoft.com/fee176ba-ad07-4145-0b4d-1b8c335fd102">POINTER_INFO</a> structure returned by a call to <a href="https://msdn.microsoft.com/75faea24-91cd-448b-b67a-19fe530f1800">GetPointerInfo</a>.


### -param pointerInfo [out, optional]

Address of an array of <a href="https://msdn.microsoft.com/fee176ba-ad07-4145-0b4d-1b8c335fd102">POINTER_INFO</a> structures to receive the pointer information. This parameter can be NULL if <i>*entriesCount</i> is zero.


## -returns



If the function succeeds, the return value is non-zero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



If the application does not process pointer input messages as fast as they are generated, some moves may be coalesced. When an application receives a coalescable pointer message, it can use the <b>GetPointerInfoHistory</b> function to retrieve information for all the individual inputs, if any, that were coalesced into the message. Note that the information retrieved is associated with the pointer message most recently retrieved by the calling thread. Once the calling thread retrieves its next message, the information associated with the previous message may no longer be available.

The information retrieved appears in reverse chronological order, with the most recent entry in the first row of the returned array. The most recent entry is the same as that returned by the <a href="https://msdn.microsoft.com/75faea24-91cd-448b-b67a-19fe530f1800">GetPointerInfo</a> function.

If the count of rows in the buffer provided is insufficient to hold all available history entries, this function succeeds with the buffer containing the most recent entries and <i>*entriesCount</i> containing the total count of entries available.


If the pointer frame contains no additional pointers besides the specified pointer, this function succeeds and returns only the information for the specified pointer.

If the information associated with the pointer frame is no longer available, this function fails with the last error set to <b>ERROR_NO_DATA</b>.

If the calling thread does not own the window (where the input was originally delivered or where the message was forwarded) to which the pointer message has been delivered, this function fails with the last error set to <b>ERROR_ACCESS_DENIED</b>. 




## -see-also




<a href="https://msdn.microsoft.com/0123DCD0-DAE1-4AC2-AB36-23D114803138">Functions</a>



<a href="https://msdn.microsoft.com/6b7f450d-6ab1-4991-b2f9-a1db3f065711">GetPointerFrameInfo</a>



<a href="https://msdn.microsoft.com/1ae035d6-a375-4421-82a6-50be4a2341f6">GetPointerFrameInfoHistory</a>



<a href="https://msdn.microsoft.com/75faea24-91cd-448b-b67a-19fe530f1800">GetPointerInfo</a>
 

 

