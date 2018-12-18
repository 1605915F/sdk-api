---
UID: NF:mswmdm.IMDSPDeviceControl.GetDCStatus
title: IMDSPDeviceControl::GetDCStatus
author: windows-sdk-content
description: The GetDCStatus method retrieves the control status of the device.
old-location: wmdm\imdspdevicecontrol_getdcstatus.htm
tech.root: WMDM
ms.assetid: 6fc51100-3052-4d26-8786-a7b1e9fe0529
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDCStatus, GetDCStatus method [windows Media Device Manager], GetDCStatus method [windows Media Device Manager],IMDSPDeviceControl interface, IMDSPDeviceControl interface [windows Media Device Manager],GetDCStatus method, IMDSPDeviceControl.GetDCStatus, IMDSPDeviceControl::GetDCStatus, IMDSPDeviceControlGetDCStatus, mswmdm/IMDSPDeviceControl::GetDCStatus, wmdm.imdspdevicecontrol_getdcstatus
ms.topic: method
req.header: mswmdm.h
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
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mssachlp.lib
 - mssachlp.dll
api_name:
 - IMDSPDeviceControl.GetDCStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMDSPDeviceControl::GetDCStatus


## -description



The <b>GetDCStatus</b> method retrieves the control status of the device.




## -parameters




### -param pdwStatus [out]

Pointer to a <b>DWORD</b> that contains the control status of the device. The control status value contains one or more of the following flags.

<table>
<tr>
<th>Flag
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>WMDM_STATUS_READY</td>
<td>Windows Media Device Manager and its subcomponents are in a ready state.</td>
</tr>
<tr>
<td>WMDM_STATUS_BUSY</td>
<td>An operation is currently being performed. Evaluate the other status values to determine which operation it is.</td>
</tr>
<tr>
<td>WMDM_STATUS_DEVICECONTROL_PLAYING</td>
<td>The device is currently playing.</td>
</tr>
<tr>
<td>WMDM_STATUS_DEVICECONTROL_RECORDING</td>
<td>The device is currently recording.</td>
</tr>
<tr>
<td>WMDM_STATUS_DEVICECONTROL_PAUSED</td>
<td>The device is currently paused.</td>
</tr>
<tr>
<td>WMDM_STATUS_DEVICECONTROL_REMOTE</td>
<td>The play or record operation of the device is being remotely controlled by the application.</td>
</tr>
<tr>
<td>WMDM_STATUS_DEVICECONTROL_STREAM</td>
<td>The play or record method is streaming data to or from the media device.</td>
</tr>
</table>
 


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>pdwStatus</i> parameter is an invalid or <b>NULL</b> pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unspecified error occurred.

</td>
</tr>
</table>
 




## -remarks



This call returns status values specific to the device control operations of this interface. The control status can provide information about the state of control-related activities of the device, such as playing, recording, and so on. However, it cannot provide information about the global status of the device, such as whether the device is downloading data or being accessed for some other reason. If the device is busy for any reason other than device control, you receive a busy code and must call the <b>GetStatus</b> method of the associated <b>IMDSPDevice</b> interface for more detailed information.

You must not attempt to call the <a href="https://msdn.microsoft.com/09ca1922-3b33-47a8-a851-a1d221a568b9">Play</a>, <a href="https://msdn.microsoft.com/6cd99cfc-1961-4369-9ce9-2cdd0136d181">Record</a>, <a href="https://msdn.microsoft.com/d97edbd0-afac-4197-b9bc-e538c2b145b2">Pause</a>, <a href="https://msdn.microsoft.com/6c7e26dc-05cd-4dfd-86c8-0b7b216b6772">Resume</a>, or <a href="https://msdn.microsoft.com/31dd1325-2a8d-4a61-a4a5-f585b320e841">Stop</a> methods of this interface if the status value WMDM_STATUS_BUSY is returned and the status value does not contain any other values from the table of status values.




## -see-also




<a href="https://msdn.microsoft.com/a196edef-f670-4c1f-92bd-172a75f3f420">IMDSPDeviceControl Interface</a>
 

 

