---
UID: NF:imapi2fs.IFsiItem.put_LastAccessedTime
title: IFsiItem::put_LastAccessedTime (imapi2fs.h)
author: windows-sdk-content
description: Sets the date and time that the directory or file item was last accessed in the file system image.
old-location: imapi\ifsiitem_put_lastaccessedtime.htm
tech.root: imapi
ms.assetid: 6192bff5-9535-4845-9c99-d5ceeea0335f
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IFsiItem interface [IMAPI],put_LastAccessedTime method, IFsiItem.put_LastAccessedTime, IFsiItem::put_LastAccessedTime, imapi.ifsiitem_put_lastaccessedtime, imapi2fs/IFsiItem::put_LastAccessedTime, put_LastAccessedTime, put_LastAccessedTime method [IMAPI], put_LastAccessedTime method [IMAPI],IFsiItem interface
ms.topic: method
req.header: imapi2fs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2fs.idl
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
 - imapi2fs.h
api_name:
 - IFsiItem.put_LastAccessedTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFsiItem::put_LastAccessedTime


## -description


Sets the date and time that the  directory or file item was last accessed in the file system image.


## -parameters




### -param newVal [in]

Date and time that the directory or file  item was last accessed in the file system image, according to UTC time. Defaults to the time the item was added to the image.


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
<dt><b>IMAPI_E_READONLY</b></dt>
</dl>
</td>
<td width="60%">
FileSystemImage object is in read only mode.

Value: 0xC0AAB102

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Failed to allocate necessary memory.

Value: 0x8007000E

</td>
</tr>
</table>
 




## -remarks



UDFS (UDF) uses the <i>LastAccessedTime</i> value for the <i>CreationTime</i>, as IMAPI does not currently support the <i>CreationTime</i> extended attribue.

CDFS (ISO 9660) sets the <i>LastAccessedTime</i> value to 0, as only the recording time is stored within the File/Directory descriptor.




## -see-also




<a href="https://msdn.microsoft.com/44494e66-e6b4-4acb-a2a6-0a3e5cc4a2a0">IFsiItem</a>



<a href="https://msdn.microsoft.com/e12f4c62-2dc8-4155-9cd7-0dea982d7b5a">IFsiItem::get_LastAccessedTime</a>
 

 

