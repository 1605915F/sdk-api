---
UID: NF:ole2.OleFlushClipboard
title: OleFlushClipboard function (ole2.h)
author: windows-sdk-content
description: Carries out the clipboard shutdown sequence. It also releases the IDataObject pointer that was placed on the clipboard by the OleSetClipboard function.
old-location: com\oleflushclipboard.htm
tech.root: com
ms.assetid: 18291a91-be7d-42ec-a44a-d1bbfb017c6e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OleFlushClipboard, OleFlushClipboard function [COM], _ole_OleFlushClipboard, com.oleflushclipboard, ole2/OleFlushClipboard
ms.topic: function
req.header: ole2.h
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
req.lib: Ole32.lib
req.dll: Ole32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ole32.dll
 - API-MS-Win-RTCore-OLE32-clipboard-l1-1-0.dll
 - ie_shims.dll
 - ext-ms-win-ole32-clipboard-ie-l1-1-0.dll
 - API-MS-Win-RTCore-Ole32-Clipboard-L1-1-1.dll
api_name:
 - OleFlushClipboard
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OleFlushClipboard function


## -description


Carries out the clipboard shutdown sequence. It also releases the <a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> pointer that was placed on the clipboard by the <a href="https://msdn.microsoft.com/741def10-d2b5-4395-8049-1eba2e29b0e8">OleSetClipboard</a> function.


## -parameters






## -returns



This function returns S_OK on success. Other possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>CLIPBRD_E_CANT_OPEN</b></dt>
</dl>
</td>
<td width="60%">
The Windows OpenClipboard function used within <a href="https://msdn.microsoft.com/18291a91-be7d-42ec-a44a-d1bbfb017c6e">OleFlushClipboard</a> failed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>CLIPBRD_E_CANT_CLOSE</b></dt>
</dl>
</td>
<td width="60%">
The Windows CloseClipboard function used within <a href="https://msdn.microsoft.com/18291a91-be7d-42ec-a44a-d1bbfb017c6e">OleFlushClipboard</a> failed.

</td>
</tr>
</table>
 




## -remarks



<b>OleFlushClipboard</b> renders the data from a data object onto the clipboard and releases the <a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> pointer to the data object. While the application that put the data object on the clipboard is running, the clipboard holds only a pointer to the data object, thus saving memory. If you are writing an application that acts as the source of a clipboard operation, you can call the <b>OleFlushClipboard</b> function when your application is closed, such as when the user exits from your application. Calling <b>OleFlushClipboard</b> enables pasting and paste-linking of OLE objects after application shutdown.

Before calling <b>OleFlushClipboard</b>, you can easily determine if your data is still on the clipboard with a call to the <a href="https://msdn.microsoft.com/12844504-ef47-4a4d-b31b-f765e0f2ace6">OleIsCurrentClipboard</a> function.

<b>OleFlushClipboard</b> leaves all formats offered by the data transfer object, including the OLE 1 compatibility formats, on the clipboard so they are available after application shutdown. In addition to OLE 1 compatibility formats, these include all formats offered on a global handle medium (all except for TYMED_FILE) and formatted with a <b>NULL</b> target device. For example, if a data-source application offers a particular clipboard format (say cfFOO) on an <a href="https://msdn.microsoft.com/2f454538-0f40-4811-b908-cd317ef79487">IStorage</a> object, and calls the <b>OleFlushClipboard</b> function, the storage object is copied into memory and the hglobal memory handle is put on the clipboard.

To retrieve the information on the clipboard, you can call the <a href="https://msdn.microsoft.com/c5e7badb-339b-48d5-8c9a-3950e2ffe6bf">OleGetClipboard</a> function from another application, which creates a default data object, and the hglobal from the clipboard again becomes a storage object. Furthermore, the <a href="https://msdn.microsoft.com/4478eb9a-84a1-4f3a-8290-94b8dd20c081">FORMATETC</a> enumerator and the <a href="https://msdn.microsoft.com/38a1bb4f-7762-4e74-a386-4ae05e59d15f">IDataObject::QueryGetData</a> method would all correctly indicate that the original clipboard format (cfFOO) is again available on a TYMED_ISTORAGE.

To empty the clipboard, call the <a href="https://msdn.microsoft.com/741def10-d2b5-4395-8049-1eba2e29b0e8">OleSetClipboard</a> function specifying a <b>NULL</b> value for its parameter. The application should call this when it closes if there is no need to leave data on the clipboard after shutdown, or if data will be placed on the clipboard using the standard Windows clipboard functions.




## -see-also




<a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a>



<a href="https://msdn.microsoft.com/c5e7badb-339b-48d5-8c9a-3950e2ffe6bf">OleGetClipboard</a>



<a href="https://msdn.microsoft.com/12844504-ef47-4a4d-b31b-f765e0f2ace6">OleIsCurrentClipboard</a>



<a href="https://msdn.microsoft.com/741def10-d2b5-4395-8049-1eba2e29b0e8">OleSetClipboard</a>
 

 

