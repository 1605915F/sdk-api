---
UID: NF:cfgmgr32.CM_Get_Device_ID_Size_Ex
title: CM_Get_Device_ID_Size_Ex function (cfgmgr32.h)
author: windows-sdk-content
description: The CM_Get_Device_ID_Size_Ex function retrieves the buffer size required to hold a device instance ID for a device instance on a local or a remote machine.
old-location: devinst\cm_get_device_id_size_ex.htm
tech.root: devinst
ms.assetid: 3b95f8e3-0059-4a2e-8c14-5938f5826faf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CM_Get_Device_ID_Size_Ex, CM_Get_Device_ID_Size_Ex function [Device and Driver Installation], cfgmgr32/CM_Get_Device_ID_Size_Ex, cfgmgrfn_c3ddb484-70bd-414f-a723-a10057ad5e19.xml, devinst.cm_get_device_id_size_ex
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
req.lib: Cfgmgr32.lib
req.dll: Cfgmgr32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Cfgmgr32.dll
api_name:
 - CM_Get_Device_ID_Size_Ex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CM_Get_Device_ID_Size_Ex function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/3ae682d0-d9fa-4a29-8258-c6f72f1940b7">CM_Get_Device_ID_Size</a> instead.]

The <b>CM_Get_Device_ID_Size_Ex</b> function retrieves the buffer size required to hold a <a href="https://msdn.microsoft.com/library/Ff541327(v=VS.85).aspx">device instance ID</a> for a <a href="https://msdn.microsoft.com/86688b5d-575d-42e1-9158-7ffba1aaf1d3">device instance</a> on a local or a remote machine.


## -parameters




### -param pulLen [out]

Receives a value representing the required buffer size, in characters.


### -param dnDevInst [in]

Caller-supplied device instance handle that is bound to the local machine.


### -param ulFlags [in]

Not used, must be zero.


### -param hMachine [in, optional]

Caller-supplied machine handle to which the caller-supplied device instance handle is bound.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



The <b>CM_Get_Device_ID_Size_Ex</b> function should be called to determine the buffer size required by <a href="https://msdn.microsoft.com/757b8185-c5f5-4623-a410-63fd2f74e34f">CM_Get_Device_ID_Ex</a>.

The size value supplied in the location pointed to by <i>pulLen</i> is less than MAX_DEVICE_ID_LEN, and does not include the identifier string's terminating <b>NULL</b>. If the specified device instance does not exist, the function supplies a size value of zero.

For information about device instance IDs, see <a href="https://docs.microsoft.com/en-us/windows-hardware/drivers/install/device-identification-strings">Device Identification Strings</a>.

For information about using device instance handles that are bound to a local or a remote machine, see <a href="https://msdn.microsoft.com/bcd46252-6f87-4d49-a24c-81789b0148d9">CM_Get_Child_Ex</a>.

 Functionality to access remote machines has been removed in Windows 8 and Windows Server 2012 and later operating systems thus you cannot access remote machines when running on these versions of Windows.




## -see-also




<a href="https://msdn.microsoft.com/bcd46252-6f87-4d49-a24c-81789b0148d9">CM_Get_Child_Ex</a>



<a href="https://msdn.microsoft.com/757b8185-c5f5-4623-a410-63fd2f74e34f">CM_Get_Device_ID_Ex</a>



<a href="https://msdn.microsoft.com/3ae682d0-d9fa-4a29-8258-c6f72f1940b7">CM_Get_Device_ID_Size</a>
 

 

