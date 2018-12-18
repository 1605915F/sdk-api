---
UID: NF:vfw.EditStreamClone
title: EditStreamClone function
author: windows-sdk-content
description: The EditStreamClone function creates a duplicate editable stream.
old-location: multimedia\editstreamclone.htm
tech.root: Multimedia
ms.assetid: 2a512dbd-8d17-43d0-a074-571b4c1837c7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EditStreamClone, EditStreamClone function [Windows Multimedia], _win32_EditStreamClone, multimedia.editstreamclone, vfw/EditStreamClone
ms.topic: function
req.header: vfw.h
req.include-header: 
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
req.lib: Vfw32.lib
req.dll: Avifil32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Avifil32.dll
api_name:
 - EditStreamClone
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# EditStreamClone function


## -description



The <b>EditStreamClone</b> function creates a duplicate editable stream.




## -parameters




### -param pavi

Handle to an editable stream that will be copied.


### -param ppResult

Pointer to a buffer that receives the new stream handle.


## -returns



Returns zero if successful or an error otherwise.




## -remarks



The editable stream that is being cloned must have been created by the <b>CreateEditableStream</b> function or one of the stream editing functions.

The new stream can be treated as any other AVI stream.




## -see-also




<a href="https://msdn.microsoft.com/89abf60a-1714-4836-93ae-a8a6bf2c24b6">AVIFile Functions</a>



<a href="https://msdn.microsoft.com/573e24fa-876d-4ce9-be23-d5e448a53e20">AVIFile Functions and Macros</a>
 

 

