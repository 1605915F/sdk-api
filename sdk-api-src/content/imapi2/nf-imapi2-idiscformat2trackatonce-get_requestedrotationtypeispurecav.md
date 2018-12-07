---
UID: NF:imapi2.IDiscFormat2TrackAtOnce.get_RequestedRotationTypeIsPureCAV
title: IDiscFormat2TrackAtOnce::get_RequestedRotationTypeIsPureCAV
author: windows-sdk-content
description: Retrieves the requested rotational-speed control type.
old-location: imapi\idiscformat2trackatonce_get_requestedrotationtypeispurecav.htm
tech.root: imapi
ms.assetid: 3702f4c1-4043-4a69-bd6b-4346c560651a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDiscFormat2TrackAtOnce interface [IMAPI],get_RequestedRotationTypeIsPureCAV method, IDiscFormat2TrackAtOnce.get_RequestedRotationTypeIsPureCAV, IDiscFormat2TrackAtOnce::get_RequestedRotationTypeIsPureCAV, get_RequestedRotationTypeIsPureCAV, get_RequestedRotationTypeIsPureCAV method [IMAPI], get_RequestedRotationTypeIsPureCAV method [IMAPI],IDiscFormat2TrackAtOnce interface, imapi.idiscformat2trackatonce_get_requestedrotationtypeispurecav, imapi2/IDiscFormat2TrackAtOnce::get_RequestedRotationTypeIsPureCAV
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
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
 - COM
api_location:
 - imapi2.h
api_name:
 - IDiscFormat2TrackAtOnce.get_RequestedRotationTypeIsPureCAV
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiscFormat2TrackAtOnce::get_RequestedRotationTypeIsPureCAV


## -description


Retrieves the requested rotational-speed control type. 


## -parameters




### -param value [out]

Requested rotational-speed control type. Is VARIANT_TRUE for constant angular velocity (CAV)  rotational-speed control type. Otherwise, is VARIANT_FALSE for any other rotational-speed control type that the recorder supports. 


## -returns



S_OK is returned on success, but other success codes may be returned as a result of implementation. The following error codes are commonly returned on operation failure, but do not represent the only possible error values:

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
Pointer is not valid.

Value: 0x80004003

</td>
</tr>
</table>
 




## -remarks



This is the value specified in the most recent call to the <a href="https://msdn.microsoft.com/29c4487a-4247-45cf-af95-dc85fafb05c5">IDiscFormat2TrackAtOnce::SetWriteSpeed</a> method.




## -see-also




<a href="https://msdn.microsoft.com/27f2d248-1c83-4784-82f9-75ce0a038b87">IDiscFormat2TrackAtOnce</a>



<a href="https://msdn.microsoft.com/29c4487a-4247-45cf-af95-dc85fafb05c5">IDiscFormat2TrackAtOnce::SetWriteSpeed</a>



<a href="https://msdn.microsoft.com/3a80eee3-6b85-432a-878c-c8e4cade7be1">IDiscFormat2TrackAtOnce::get_CurrentRotationTypeIsPureCAV</a>
 

 

