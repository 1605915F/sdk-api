---
UID: NF:wmsdkidl.WMCreateSyncReader
title: WMCreateSyncReader function
author: windows-sdk-content
description: The WMCreateSyncReader function creates a synchronous reader object.
old-location: wmformat\wmcreatesyncreader.htm
tech.root: wmformat
ms.assetid: 77cb65cc-9785-4af4-9b92-245c17e5ab82
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WMCreateSyncReader, WMCreateSyncReader function [windows Media Format], wmformat.wmcreatesyncreader, wmsdkidl/WMCreateSyncReader
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
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
req.lib: Wmvcore.lib
req.dll: Wmvcore.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Wmvcore.dll
api_name:
 - WMCreateSyncReader
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WMCreateSyncReader function


## -description



The <b>WMCreateSyncReader</b> function creates a synchronous reader object.




## -parameters




### -param pUnkCert [in]

Pointer to an <b>IUnknown</b> interface. This value must be set to <b>NULL</b>.


### -param dwRights [in]

<b>DWORD</b> specifying the desired operation. When playing back non-DRM content, or for an application that does not have DRM rights, this value can be set to zero. Otherwise, this value must be one of the values from the <a href="https://msdn.microsoft.com/52a9a5ec-58fb-4804-8f56-4d863c738934">WMT_RIGHTS</a> enumeration type, indicating the operation that is performed on this file. If multiple operations are being performed, <b>dwRights</b> must consist of multiple values from <b>WMT_RIGHTS</b> combined by using the bitwise <b>OR</b> operator.


### -param ppSyncReader [out]

Pointer to a pointer to the <a href="https://msdn.microsoft.com/2a46e79f-084e-4173-ad0f-211d3065d81a">IWMSyncReader</a> interface of the newly created synchronous reader object.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The function succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The function is unable to allocate memory for the new object.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/10fa8f96-8030-4727-af5d-7c06229d05d8">Functions</a>



<a href="https://msdn.microsoft.com/52a4891f-03bf-4d8a-ab7b-e9739db30bc3">Synchronous Reader Object</a>
 

 

