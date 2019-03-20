---
UID: NS:objidl.tagSTATSTG
title: STATSTG (objidl.h)
author: windows-sdk-content
description: Contains statistical data about an open storage, stream, or byte-array object.
old-location: stg\statstg.htm
tech.root: Stg
ms.assetid: 54e1df08-de8f-430a-bf76-e66594df4839
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: STATSTG, STATSTG [Strctd Stg], STATSTG structure [Structured Storage], _stg_statstg, objidl/STATSTG, stg.statstg, tagSTATSTG
ms.topic: struct
req.header: objidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
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
 - Objidl.h
api_name:
 - STATSTG
product: Windows
targetos: Windows
req.typenames: STATSTG
req.redist: 
---

# STATSTG structure


## -description


The 
<b>STATSTG</b> structure contains statistical data about an open storage, stream, or byte-array object. This structure is used in the 
<a href="https://msdn.microsoft.com/93b8b14e-94e4-460b-9846-413affad8e4f">IEnumSTATSTG</a>, 
<a href="https://msdn.microsoft.com/bb2c5d0d-8dc8-4844-9a20-ef8e4def5731">ILockBytes</a>, 
<a href="https://msdn.microsoft.com/2f454538-0f40-4811-b908-cd317ef79487">IStorage</a>, and 
<a href="https://msdn.microsoft.com/c6f60e37-eadc-46a1-94f6-cacc23613531">IStream</a> interfaces.


## -struct-fields




### -field pwcsName

A pointer to a <b>NULL</b>-terminated Unicode string that contains the name. Space for this string is allocated by the method called and freed by the caller (for more information, see 
<a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a>). To  not return this member, specify the STATFLAG_NONAME value when you call a method that returns a 
<b>STATSTG</b> structure, except for calls to <a href="https://msdn.microsoft.com/93b8b14e-94e4-460b-9846-413affad8e4f">IEnumSTATSTG::Next</a>, which provides no way to specify this value.


### -field type

Indicates the type of storage object. This is one of the values from the 
<a href="https://msdn.microsoft.com/67189e7a-b089-4a29-adf8-ad7c459c7974">STGTY</a> enumeration.


### -field cbSize

Specifies the size, in bytes, of the stream or byte array.


### -field mtime

Indicates the last modification time for this storage, stream, or byte array.


### -field ctime

Indicates the creation time for this storage, stream, or byte array.


### -field atime

Indicates the last access time for this storage, stream, or byte array.


### -field grfMode

Indicates the access mode specified when the object was opened. This member is only valid in calls to 
<b>Stat</b> methods.


### -field grfLocksSupported

Indicates the types of region locking supported by the stream or byte array. For more information about the values available, see the 
<a href="https://msdn.microsoft.com/5d84fb08-aa4f-4918-a0de-550b02cb5287">LOCKTYPE</a> enumeration. This member is not used for storage objects.


### -field clsid

Indicates the class identifier for the storage object; set to CLSID_NULL for new storage objects. This member is not used for streams or byte arrays.


### -field grfStateBits

Indicates the current state bits of the storage object; that is, the value most recently set by the 
<a href="https://msdn.microsoft.com/52606df8-10ea-40e7-bb61-c86c7b7262d2">IStorage::SetStateBits</a> method. This member is not valid for streams or byte arrays.


### -field reserved

Reserved for future use.


## -see-also




<a href="https://msdn.microsoft.com/f6a1fba4-0444-4de3-a838-2d339878fe24">IStorage::SetElementTimes</a>
 

 

