---
UID: NE:objidlbase._THDTYPE
title: THDTYPE (objidlbase.h)
author: windows-sdk-content
description: Indicates whether a particular thread supports a message loop.
old-location: com\thdtype.htm
tech.root: com
ms.assetid: c1f9ab7b-8915-4433-ae9f-57b1aedcad4d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: THDTYPE, THDTYPE enumeration [COM], THDTYPE_BLOCKMESSAGES, THDTYPE_PROCESSMESSAGES, _com_THDTYPE, com.thdtype, objidlbase/THDTYPE, objidlbase/THDTYPE_BLOCKMESSAGES, objidlbase/THDTYPE_PROCESSMESSAGES
ms.topic: enum
req.header: objidlbase.h
req.include-header: Objidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - objidlbase.h
api_name:
 - THDTYPE
product: Windows
targetos: Windows
req.typenames: THDTYPE
req.redist: 
---

# THDTYPE enumeration


## -description


Indicates whether a particular thread supports a message loop.


## -enum-fields




### -field THDTYPE_BLOCKMESSAGES

The thread does not support a message loop. This behavior is associated with multithreaded apartments.


### -field THDTYPE_PROCESSMESSAGES

The thread supports a message loop. This behavior is associated with single-threaded apartments.


## -see-also




<a href="https://msdn.microsoft.com/93437e45-f1e7-4f1f-bffb-ef234c7f5a6b">IComThreadingInfo::GetCurrentThreadType</a>
 

 

