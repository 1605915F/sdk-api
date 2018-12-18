---
UID: NS:xinput._XINPUT_VIBRATION
title: XINPUT_VIBRATION
author: windows-sdk-content
description: Specifies motor speed levels for the vibration function of a controller.
old-location: xinput\xinput_vibration.htm
tech.root: xinput
ms.assetid: T:Microsoft.directx_sdk.reference.XINPUT_VIBRATION
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PXINPUT_VIBRATION, PXINPUT_VIBRATION, PXINPUT_VIBRATION structure pointer [XInput Game Controller APIs], XINPUT_VIBRATION, XINPUT_VIBRATION structure [XInput Game Controller APIs], xinput.xinput_vibration, xinput/PXINPUT_VIBRATION, xinput/XINPUT_VIBRATION"
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - XInput.h
api_name:
 - XINPUT_VIBRATION
product: Windows
targetos: Windows
req.typenames: XINPUT_VIBRATION, *PXINPUT_VIBRATION
req.redist: 
---

# XINPUT_VIBRATION structure


## -description


Specifies motor speed levels for the vibration function of a controller.


## -struct-fields




### -field wLeftMotorSpeed

Speed of the left motor. Valid values are in the range 0 to 65,535. Zero signifies no motor use; 65,535 signifies 100 percent motor use.


### -field wRightMotorSpeed

Speed of the right motor. Valid values are in the range 0 to 65,535. Zero signifies no motor use; 65,535 signifies 100 percent motor use.


## -remarks



The left motor is the low-frequency rumble motor. The right motor is the high-frequency rumble motor. The two motors are not the same, and they create different vibration effects.




## -see-also




<a href="https://msdn.microsoft.com/9F3BA764-82E0-4C46-AAA3-F417D2344ECB">XINPUT_GAMEPAD</a>



<a href="https://msdn.microsoft.com/89bb00ea-0be3-9619-1629-a7b7894302d5">XInput Structures</a>



<a href="https://msdn.microsoft.com/5F02EFF5-57ED-4FF1-88E2-DB1CB6F33151">XInputGetCapabilities</a>



<a href="https://msdn.microsoft.com/FA494AEB-9FB9-4AF4-95AB-01048A60D924">XInputSetState</a>
 

 

