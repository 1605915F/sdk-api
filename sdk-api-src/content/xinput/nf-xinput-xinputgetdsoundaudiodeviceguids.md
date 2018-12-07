---
UID: NF:xinput.XInputGetDSoundAudioDeviceGuids
title: XInputGetDSoundAudioDeviceGuids function
author: windows-sdk-content
description: Gets the sound rendering and sound capture device GUIDs that are associated with the headset connected to the specified controller.
old-location: xinput\xinputgetdsoundaudiodeviceguids.htm
tech.root: xinput
ms.assetid: M:Microsoft.directx_sdk.reference.XInputGetDSoundAudioDeviceGuids(DWORD,GUID*@,GUID*@)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XInputGetDSoundAudioDeviceGuids, XInputGetDSoundAudioDeviceGuids function [XInput Game Controller APIs], xinput.xinputgetdsoundaudiodeviceguids, xinput/XInputGetDSoundAudioDeviceGuids
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: xinput.h
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
req.lib: Xinput.lib; Xinput9_1_0.lib
req.dll: Xinput9_1_0.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - xinput9_1_0.dll
api_name:
 - XInputGetDSoundAudioDeviceGuids
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XInputGetDSoundAudioDeviceGuids function


## -description


Gets the sound rendering and sound capture device GUIDs that are associated with the headset connected to the specified controller.


## -parameters




### -param dwUserIndex

[in] Index of the user's controller. It can be a value in the range 0–3. For information about how this value is determined and how the value maps to indicators on the controller, see <a href="https://msdn.microsoft.com/en-us/library/Ee417001(v=VS.85).aspx">Multiple Controllers</a>.


### -param pDSoundRenderGuid

[out] Pointer that receives the GUID of the headset sound rendering device.


### -param pDSoundCaptureGuid

[out] Pointer that receives the GUID of the headset sound capture device.


## -returns



If the function successfully retrieves the device IDs for render and capture, the return code is <b>ERROR_SUCCESS</b>.



If there is no headset connected to the controller, the function also retrieves <b>ERROR_SUCCESS</b> with <b>GUID_NULL</b> as the values for <i>pDSoundRenderGuid</i> and <i>pDSoundCaptureGuid</i>.



If the controller port device is not physically connected, the function returns <b>ERROR_DEVICE_NOT_CONNECTED</b>.



If the function fails, it returns a valid Win32 error code.





## -remarks



Use of legacy <a href="https://msdn.microsoft.com/library/Ee416960(v=VS.85).aspx">DirectSound</a> is not recommended, and DirectSound is not available for Windows Store apps.

<div class="alert"><b>Note</b>  <b>XInputGetDSoundAudioDeviceGuids</b> is deprecated because it isn't supported by Windows 8 (XInput 1.4).</div>
<div> </div>
<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
DirectX SDK (XInput 1.3), Windows Vista (XInput 9.1.0)




## -see-also




<a href="https://msdn.microsoft.com/c1533555-9094-0030-f025-6f47e9002e1a">XInput Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee419267(v=VS.85).aspx">XInputGetState</a>
 

 

