---
UID: NF:objidl.IPersistStorage.SaveCompleted
title: IPersistStorage::SaveCompleted (objidl.h)
author: windows-sdk-content
description: Notifies the object that it can write to its storage object.
old-location: com\ipersiststorage_savecompleted.htm
tech.root: com
ms.assetid: 18c223e7-38ce-4f20-818b-84bd4c7e0dfd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPersistStorage interface [COM],SaveCompleted method, IPersistStorage.SaveCompleted, IPersistStorage::SaveCompleted, SaveCompleted, SaveCompleted method [COM], SaveCompleted method [COM],IPersistStorage interface, _com_ipersiststorage_savecompleted, com.ipersiststorage_savecompleted, objidl/IPersistStorage::SaveCompleted
ms.topic: method
req.header: objidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ObjIdl.idl
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
 - ObjIdl.h
api_name:
 - IPersistStorage.SaveCompleted
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPersistStorage::SaveCompleted


## -description


Notifies the object that it can write to its storage object. It does this by notifying the object that it can revert from NoScribble mode (in which it must not write to its storage object), to Normal mode (in which it can). The object enters NoScribble mode when it receives an <a href="https://msdn.microsoft.com/3a200812-48d9-4202-987a-1400aa66191c">IPersistStorage::Save</a> call.


## -parameters




### -param pStgNew [in]

An <a href="https://msdn.microsoft.com/2f454538-0f40-4811-b908-cd317ef79487">IStorage</a> pointer to the new storage object, if different from the storage object prior to saving. This pointer can be <b>NULL</b> if the current storage object does not change during the save operation. If the object is in HandsOff mode, this parameter must be non-<b>NULL</b>.


## -returns



This method can return the following values.

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
The method completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The object remained in HandsOff mode or NoScribble mode due to a lack of memory. Typically, this error occurs when the object is not able to open the necessary streams and storage objects in <i>pStgNew</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>pStgNew</i> parameter is not valid. Typically, this error occurs if <i>pStgNew</i> is <b>NULL</b> when the object is in HandsOff mode.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
The object is in Normal mode, and there was no previous call to <a href="https://msdn.microsoft.com/3a200812-48d9-4202-987a-1400aa66191c">IPersistStorage::Save</a> or <a href="https://msdn.microsoft.com/1e5ef26f-d8e7-4fa6-bfc4-19dace35314d">IPersistStorage::HandsOffStorage</a>. 


</td>
</tr>
</table>
 




## -remarks



This method notifies an object that it can revert to Normal mode and can once again write to its storage object. The object exits NoScribble mode or HandsOff mode.

If the object is reverting from HandsOff mode, the pStgNew parameter must be non-<b>NULL</b>. In HandsOffFromNormal mode, this parameter is the new storage object that replaces the one that was revoked by the <a href="https://msdn.microsoft.com/1e5ef26f-d8e7-4fa6-bfc4-19dace35314d">IPersistStorage::HandsOffStorage</a> method. The data in the storage object is a copy of the data from the revoked storage object. In HandsOffAfterSave mode, the data is the same as the data that was most recently saved. It is not the same as the data in the revoked storage object.

If the object is reverting from NoScribble mode, the <i>pStgNew</i> parameter can be <b>NULL</b> or non-<b>NULL</b>. If <b>NULL</b>, the object once again has access to its storage object. If it is not <b>NULL</b>, the component object should simulate receiving a call to its <a href="https://msdn.microsoft.com/1e5ef26f-d8e7-4fa6-bfc4-19dace35314d">HandsOffStorage</a> method. If the component object cannot simulate this call, its container must be prepared to actually call the <b>HandsOffStorage</b> method.

This method must recursively call any nested objects that are loaded or running.

If this method returns an error code, the object is not returned to Normal mode. Thus, the container object can attempt different save strategies.




## -see-also




<a href="https://msdn.microsoft.com/1c1a20fc-c101-4cbc-a7a6-30613aa387d7">IPersistStorage</a>
 

 

