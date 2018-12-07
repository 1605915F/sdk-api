---
UID: NS:bcrypt._BCryptBufferDesc
title: "_BCryptBufferDesc"
author: windows-sdk-content
description: Used to receieve a collection of NCryptBuffer structures.
old-location: security\ncryptbufferdesc_struct.htm
tech.root: seccng
ms.assetid: ae4673ab-81cd-4604-bafa-8d8c66003aba
ms.author: windowssdkdev
ms.date: 10/12/2018
ms.keywords: "*PBCryptBufferDesc, BCryptBufferDesc, NCRYPTBUFFER_VERSION, NCryptBufferDesc, NCryptBufferDesc structure [Security], PNCryptBufferDesc, PNCryptBufferDesc structure pointer [Security], _BCryptBufferDesc, bcrypt/NCryptBufferDesc, bcrypt/PNCryptBufferDesc, security.ncryptbufferdesc_struct"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bcrypt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - Bcrypt.h
api_name:
 - NCryptBufferDesc
product: Windows
targetos: Windows
req.typenames: BCryptBufferDesc, *PBCryptBufferDesc
req.redist: 
---

# _BCryptBufferDesc structure


## -description


The <b>NCryptBufferDesc</b> structure is used to receieve a collection of <a href="https://msdn.microsoft.com/en-us/library/Aa376245(v=VS.85).aspx">NCryptBuffer</a> structures.


## -struct-fields




### -field ulVersion

The version number of the structure. Currently, this member must be the following value.



#### NCRYPTBUFFER_VERSION (0)


### -field cBuffers

The number of elements in the <b>pBuffers</b> array. You can test the value received against <b>NCRYPTBUFFER_EMPTY</b> (0) to determine whether the array pointed to by the <b>pBuffers</b> parameter contains any members.


### -field pBuffers

An array of <a href="https://msdn.microsoft.com/en-us/library/Aa376245(v=VS.85).aspx">NCryptBuffer</a> structures that contain the buffer information. The <b>cBuffers</b> member contains the number of elements in this array.


## -remarks



BCryptBufferDesc is an alias for this structure.




## -see-also




<a href="https://msdn.microsoft.com/1588eb29-4026-4d1c-8bee-a035df38444a">NCryptExportKey</a>
 

 

