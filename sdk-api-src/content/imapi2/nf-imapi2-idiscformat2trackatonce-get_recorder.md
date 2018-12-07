---
UID: NF:imapi2.IDiscFormat2TrackAtOnce.get_Recorder
title: IDiscFormat2TrackAtOnce::get_Recorder
author: windows-sdk-content
description: Retrieves the recording device to use for the write operation.
old-location: imapi\idiscformat2trackatonce_get_recorder.htm
tech.root: imapi
ms.assetid: 62a60ffb-4a9b-4921-b7fa-acc5a439e92b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDiscFormat2TrackAtOnce interface [IMAPI],get_Recorder method, IDiscFormat2TrackAtOnce.get_Recorder, IDiscFormat2TrackAtOnce::get_Recorder, get_Recorder, get_Recorder method [IMAPI], get_Recorder method [IMAPI],IDiscFormat2TrackAtOnce interface, imapi.idiscformat2trackatonce_get_recorder, imapi2/IDiscFormat2TrackAtOnce::get_Recorder
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
 - IDiscFormat2TrackAtOnce.get_Recorder
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiscFormat2TrackAtOnce::get_Recorder


## -description


Retrieves the recording device to use for the write operation.


## -parameters




### -param value [out]

An <a href="https://msdn.microsoft.com/34f858b8-74eb-4725-8815-7954cb98cff0">IDiscRecorder2</a> interface that identifies the recording device to use in the write operation.


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
 




## -see-also




<a href="https://msdn.microsoft.com/27f2d248-1c83-4784-82f9-75ce0a038b87">IDiscFormat2TrackAtOnce</a>



<a href="https://msdn.microsoft.com/6d67b076-0c3f-4d1f-aa19-8e22dd98f331">IDiscFormat2TrackAtOnce::put_Recorder</a>
 

 

