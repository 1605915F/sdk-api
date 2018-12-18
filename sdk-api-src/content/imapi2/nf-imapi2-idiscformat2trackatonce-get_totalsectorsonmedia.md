---
UID: NF:imapi2.IDiscFormat2TrackAtOnce.get_TotalSectorsOnMedia
title: IDiscFormat2TrackAtOnce::get_TotalSectorsOnMedia
author: windows-sdk-content
description: Retrieves the total sectors available on the media if writing one continuous audio track.
old-location: imapi\idiscformat2trackatonce_get_totalsectorsonmedia.htm
tech.root: imapi
ms.assetid: 86af52be-d1ea-4ccb-b1b4-e301d70cac53
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDiscFormat2TrackAtOnce interface [IMAPI],get_TotalSectorsOnMedia method, IDiscFormat2TrackAtOnce.get_TotalSectorsOnMedia, IDiscFormat2TrackAtOnce::get_TotalSectorsOnMedia, get_TotalSectorsOnMedia, get_TotalSectorsOnMedia method [IMAPI], get_TotalSectorsOnMedia method [IMAPI],IDiscFormat2TrackAtOnce interface, imapi.idiscformat2trackatonce_get_totalsectorsonmedia, imapi2/IDiscFormat2TrackAtOnce::get_TotalSectorsOnMedia
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
 - IDiscFormat2TrackAtOnce.get_TotalSectorsOnMedia
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiscFormat2TrackAtOnce::get_TotalSectorsOnMedia


## -description


Retrieves the total sectors available on the media if writing one continuous audio track.


## -parameters




### -param value [out]

Number of all sectors on the media that can be used for audio if one continuous audio track was recorded.


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
<tr>
<td width="40%">
<dl>
<dt><b>E_IMAPI_DF2TAO_MEDIA_IS_NOT_PREPARED</b></dt>
</dl>
</td>
<td width="60%">
The media is not prepared (IDiscFormat2TrackAtOnce::PrepareMedia has not been called).

Value: 0xC0AA0502

</td>
</tr>
</table>
 




## -remarks



This property can be retrieved at any time; however, during writing, the value  is cached.




## -see-also




<a href="https://msdn.microsoft.com/33313831-859c-4e35-9a43-cde2220b43d1">IDiscFormat2Data::get_FreeSectorsOnMedia</a>



<a href="https://msdn.microsoft.com/9ad23657-36db-4edd-841d-eecb591209f5">IDiscFormat2Data::get_TotalSectorsOnMedia</a>



<a href="https://msdn.microsoft.com/27f2d248-1c83-4784-82f9-75ce0a038b87">IDiscFormat2TrackAtOnce</a>



<a href="https://msdn.microsoft.com/a36dd3de-ca08-4783-beca-95813402692b">IDiscFormat2TrackAtOnce::get_FreeSectorsOnMedia</a>



<a href="https://msdn.microsoft.com/85bbb2a8-6ff9-4af4-aefd-fca85f727f37">IDiscFormat2TrackAtOnce::get_UsedSectorsOnMedia</a>
 

 

