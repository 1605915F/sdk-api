---
UID: NC:resapi.PBEGIN_RESCALL_ROUTINE
title: PBEGIN_RESCALL_ROUTINE
author: windows-sdk-content
description: Starts a call to a resource control code. The PBEGIN_RESCALL_ROUTINE type defines a pointer to this callback function.
old-location: mscs\beginresourcecontrol.htm
tech.root: mscs
ms.assetid: 1B95607F-658A-469D-8935-DF7E537D1509
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BeginResourceControl, BeginResourceControl callback, BeginResourceControl callback function [Failover Cluster], PBEGIN_RESCALL_ROUTINE, PBEGIN_RESCALL_ROUTINE callback function [Failover Cluster], mscs.beginresourcecontrol, resapi/BeginResourceControl, resapi/PBEGIN_RESCALL_ROUTINE
ms.topic: callback
req.header: resapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012 R2
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
 - ResApi.h
api_name:
 - BeginResourceControl
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PBEGIN_RESCALL_ROUTINE callback function


## -description


Starts a call to a resource control code. The <b>PBEGIN_RESCALL_ROUTINE</b> type defines a pointer to this callback function.


## -parameters




### -param Resource [in]

The resource ID for the resource.


### -param ControlCode [in]

The control code to call.


### -param InBuffer [in]

A pointer to the buffer that contains the input data for the call to the control code.


### -param InBufferSize [in]

The size of the buffer specified by <i>InBuffer</i>, in bytes.


### -param OutBuffer [out]

A pointer to the buffer that contains the output data for the call to the control code.


### -param OutBufferSize [in]

The size of the buffer specified by <i>OutBuffer</i>, in bytes.


### -param BytesReturned [out]

The size of the data returned by <i>OutBuffer</i>, in bytes.


### -param context [in]

The context to the resource control code that was called.

<b>Windows Server 2012 R2:  </b>This parameter was added in Windows Server 2016.


### -param ReturnedAsynchronously [out]

<b>TRUE</b> if the operation returns asynchronously; otherwise, <b>FALSE</b>.

<b>Windows Server 2012 R2:  </b>This parameter was added in Windows Server 2016.


#### - resCallId [in]

This parameter was removed in Windows Server 2016.

<b>Windows Server 2012 R2:  </b>This parameter is only supported in Windows Server 2012 R2.


## -returns



The function returns one of the following values, or a system error code:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
The operation completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_RESOURCE_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The resource ID was not found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_FUNCTION</b></dt>
</dl>
</td>
<td width="60%">
The requested control code is not supported.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/71ec60fd-67ec-4932-983b-f78c6b552954">Resource Control Codes</a>



<a href="https://msdn.microsoft.com/933d7b97-b5be-4c84-a983-41d1fd935c19">Resource DLL Entry-Point Functions</a>
 

 

