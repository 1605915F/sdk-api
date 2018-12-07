---
UID: NC:cchannel.VIRTUALCHANNELWRITE
title: VIRTUALCHANNELWRITE
author: windows-sdk-content
description: Sends data from the client end of a virtual channel to a partner application on the server end.
old-location: termserv\virtualchannelwrite.htm
tech.root: termserv
ms.assetid: bd7bc65e-403c-4e29-bdb4-f2f5a957d6ab
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: VirtualChannelWrite, VirtualChannelWrite callback, VirtualChannelWrite callback function [Remote Desktop Services], _win32_virtualchannelwrite, cchannel/VirtualChannelWrite, termserv.virtualchannelwrite
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: cchannel.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Cchannel.h
api_name:
 - VirtualChannelWrite
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# VIRTUALCHANNELWRITE callback function


## -description


Sends data from the client end of a virtual channel to a partner application on the server end.

Remote Desktop Services provides a pointer to a 
<b>VirtualChannelWrite</b> function in the 
<a href="https://msdn.microsoft.com/en-us/library/Aa380779(v=VS.85).aspx">CHANNEL_ENTRY_POINTS</a> structure passed to your 
<a href="https://msdn.microsoft.com/en-us/library/Aa383560(v=VS.85).aspx">VirtualChannelEntry</a> entry point.


## -parameters




### -param openHandle [in]

Handle to the virtual channel. This is the handle returned in the <i>pOpenHandle</i> parameter of the 
<a href="https://msdn.microsoft.com/en-us/library/Aa383570(v=VS.85).aspx">VirtualChannelOpen</a> function.


### -param pData [in]

Pointer to a buffer containing the data to write.


### -param dataLength [in]

Specifies the number of bytes of the data in the <i>pData</i> buffer to write.


### -param pUserData [in]

An application-defined value. This value is passed to your 
<a href="https://msdn.microsoft.com/en-us/library/Aa383573(v=VS.85).aspx">VirtualChannelOpenEvent</a> function when the write operation is completed or canceled.


## -returns



If the function succeeds, the return value is CHANNEL_RC_OK.

If an error occurs, the function returns one of the following values.




## -remarks



The 
<b>VirtualChannelWrite</b> function is asynchronous. When the write operation has been completed, your 
<a href="https://msdn.microsoft.com/en-us/library/Aa383573(v=VS.85).aspx">VirtualChannelOpenEvent</a> function receives a CHANNEL_EVENT_WRITE_COMPLETE notification. Until that notification is received, the caller must not free or reuse the <i>pData</i> buffer passed to 
<b>VirtualChannelWrite</b>.

The value specified for the <i>pUserData</i> parameter is passed to your 
<b>VirtualChannelOpenEvent</b> function when the write operation is completed or canceled. You can use this data to identify the write operation.

The server add-in at the server end of the virtual channel calls the 
<a href="https://msdn.microsoft.com/en-us/library/Aa383853(v=VS.85).aspx">WTSVirtualChannelRead</a> function to read the data written by a 
<b>VirtualChannelWrite</b> call.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa383570(v=VS.85).aspx">VirtualChannelOpen</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa383573(v=VS.85).aspx">VirtualChannelOpenEvent</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa383853(v=VS.85).aspx">WTSVirtualChannelRead</a>
 

 

