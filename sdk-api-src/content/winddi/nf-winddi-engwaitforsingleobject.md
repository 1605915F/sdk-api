---
UID: NF:winddi.EngWaitForSingleObject
title: EngWaitForSingleObject function (winddi.h)
author: windows-sdk-content
description: The EngWaitForSingleObject function puts the current thread of the display driver into a wait state until the specified event object is set to the signaled state, or until the wait times out.
old-location: display\engwaitforsingleobject.htm
tech.root: display
ms.assetid: a2a1c7ad-1e56-45f7-83de-49ebc0d831f9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EngWaitForSingleObject, EngWaitForSingleObject function [Display Devices], display.engwaitforsingleobject, gdifncs_12c16d6b-ff3f-4cd4-8d4c-150ab8377dfb.xml, winddi/EngWaitForSingleObject
ms.topic: function
req.header: winddi.h
req.include-header: Winddi.h
req.target-type: Universal
req.target-min-winverclnt: This function is available in Windows XP and later.
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
req.lib: Win32k.lib
req.dll: Win32k.sys
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Win32k.sys
api_name:
 - EngWaitForSingleObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# EngWaitForSingleObject function


## -description


The <b>EngWaitForSingleObject</b> function puts the current thread of the display driver into a wait state until the specified event object is set to the signaled state, or until the wait times out.


## -parameters




### -param pEvent [in]

Pointer to an initialized event object. This event object handle was obtained in a previous call to <a href="https://msdn.microsoft.com/0fe4c840-ba85-492c-ac3d-b7c8639d1210">EngCreateEvent</a>.


### -param pTimeOut [in]

(<i>Optional</i>) Pointer to a time-out value that specifies the absolute or relative time at which the wait is to be completed. A negative value specifies an interval relative to the current time. The value should be expressed in units of 100 nanoseconds. Absolute expiration times track any changes in the system time; relative expiration times are not affected by system time changes. If <i>pTimeOut</i> is <b>NULL</b>, the calling thread remains in a waiting state until the event object is signaled.


## -returns



<b>EngWaitForSingleObject</b> returns <b>TRUE</b> upon success, which includes the occurrence of a time-out. Otherwise, it returns <b>FALSE</b>. A return value of <b>FALSE</b> indicates that one of the parameters is invalid.




## -remarks



<b>EngWaitForSingleObject</b> causes a display driver thread to be put into a wait state. The display driver thread stays in the wait state until either the event object is set to the signaled state or until the wait times out. If no time-out value is supplied, the display driver thread remains in the wait state until the event object is set to the signaled state.

A synchronization event is automatically reset to the nonsignaled state when the wait is satisfied. Thus, only one wait will be satisfied per call to <a href="https://msdn.microsoft.com/04e5d5e0-02b1-4335-9830-ecf04fdc0db1">EngSetEvent</a> or <a href="https://msdn.microsoft.com/93db9d51-3f80-47ff-a2c2-3c937b5dcf7b">VideoPortSetEvent</a>. In contrast, a notification event will not be automatically reset.

A time-out value of zero allows the driver to test the wait condition and to conditionally perform any side effects provided that the wait can be immediately satisfied.

The display driver can synchronize drawing operations between itself and the video miniport driver by calling <b>EngWaitForSingleObject</b> with an event object, and waiting until the miniport driver sets the event object to the signaled state.

The driver cannot call <b>EngWaitForSingleObject</b> on events returned from <a href="https://msdn.microsoft.com/a48f2367-49da-4d5c-87e5-b5c67e2311eb">EngMapEvent</a>.




## -see-also




<a href="https://msdn.microsoft.com/0fe4c840-ba85-492c-ac3d-b7c8639d1210">EngCreateEvent</a>



<a href="https://msdn.microsoft.com/04e5d5e0-02b1-4335-9830-ecf04fdc0db1">EngSetEvent</a>



<a href="https://msdn.microsoft.com/93db9d51-3f80-47ff-a2c2-3c937b5dcf7b">VideoPortSetEvent</a>
 

 

