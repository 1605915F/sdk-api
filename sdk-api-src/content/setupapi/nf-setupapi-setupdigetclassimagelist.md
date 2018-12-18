---
UID: NF:setupapi.SetupDiGetClassImageList
title: SetupDiGetClassImageList function
author: windows-sdk-content
description: The SetupDiGetClassImageList function builds an image list that contains bitmaps for every installed class and returns the list in a data structure.
old-location: devinst\setupdigetclassimagelist.htm
tech.root: devinst
ms.assetid: d6b84403-9284-4fba-a419-a013cf68ea1e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetupDiGetClassImageList, SetupDiGetClassImageList function [Device and Driver Installation], devinst.setupdigetclassimagelist, di-rtns_ef2c4660-f78a-4228-9b24-9c84e38765e5.xml, setupapi/SetupDiGetClassImageList
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Setupapi.dll
api_name:
 - SetupDiGetClassImageList
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetupDiGetClassImageList function


## -description


The <b>SetupDiGetClassImageList</b> function builds an image list that contains bitmaps for every installed class and returns the list in a data structure.


## -parameters




### -param ClassImageListData [out]

A pointer to an <a href="https://msdn.microsoft.com/89ed9dbd-3c5e-43ff-bbd0-fd6cc8c6e6ab">SP_CLASSIMAGELIST_DATA</a> structure to receive information regarding the class image list, including a handle to the image list. The <b>cbSize</b> field of this structure must be initialized with the size of the structure, in bytes, before calling this function or it will fail.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved by a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



The image list built by this function should be destroyed by calling <a href="https://msdn.microsoft.com/47ccc16c-b061-489b-b534-5b5929c5d010">SetupDiDestroyClassImageList</a>.

Call <a href="https://msdn.microsoft.com/f9cf7904-3fda-4f7f-bb05-3634fd1c9af3">SetupDiGetClassImageListEx</a> to retrieve the image list for classes installed on a remote computer.




## -see-also




<a href="https://msdn.microsoft.com/47ccc16c-b061-489b-b534-5b5929c5d010">SetupDiDestroyClassImageList</a>



<a href="https://msdn.microsoft.com/f9cf7904-3fda-4f7f-bb05-3634fd1c9af3">SetupDiGetClassImageListEx</a>
 

 

