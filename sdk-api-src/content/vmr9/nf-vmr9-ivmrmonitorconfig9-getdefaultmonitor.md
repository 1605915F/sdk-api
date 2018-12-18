---
UID: NF:vmr9.IVMRMonitorConfig9.GetDefaultMonitor
title: IVMRMonitorConfig9::GetDefaultMonitor
author: windows-sdk-content
description: The GetDefaultMonitor method retrieves the default monitor that all future instances of the VMR will use for video playback.
old-location: dshow\ivmrmonitorconfig9_getdefaultmonitor.htm
tech.root: DirectShow
ms.assetid: a5d5bf77-5261-42eb-b79b-d72dfb2d9f21
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDefaultMonitor, GetDefaultMonitor method [DirectShow], GetDefaultMonitor method [DirectShow],IVMRMonitorConfig9 interface, IVMRMonitorConfig9 interface [DirectShow],GetDefaultMonitor method, IVMRMonitorConfig9.GetDefaultMonitor, IVMRMonitorConfig9::GetDefaultMonitor, IVMRMonitorConfig9GetDefaultMonitor, dshow.ivmrmonitorconfig9_getdefaultmonitor, vmr9/IVMRMonitorConfig9::GetDefaultMonitor
ms.topic: method
req.header: vmr9.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IVMRMonitorConfig9.GetDefaultMonitor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVMRMonitorConfig9::GetDefaultMonitor


## -description



The <code>GetDefaultMonitor</code> method retrieves the default monitor that all future instances of the VMR will use for video playback.




## -parameters




### -param puDev [out]

Pointer that receives an index that identifies the default monitor on the system.


## -returns



The method returns an <b>HRESULT</b>. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<b>NULL</b> pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VFW_E_WRONG_STATE</b></dt>
</dl>
</td>
<td width="60%">
The allocator-presenter has not been loaded.

</td>
</tr>
</table>
 




## -remarks



Use this method on a multi-monitor system to determine which is the default Direct3D device the overlay mixer filter will use when connecting to an upstream filter.

Include DShow.h and D3d9.h before Vmr9.h.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd390482(v=VS.85).aspx">IVMRMonitorConfig9 Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd390486(v=VS.85).aspx">IVMRMonitorConfig9::SetDefaultMonitor</a>



<a href="https://msdn.microsoft.com/3d0fdfac-ec7e-4e02-886b-2039c607dac7">Using the Video Mixing Renderer</a>
 

 

