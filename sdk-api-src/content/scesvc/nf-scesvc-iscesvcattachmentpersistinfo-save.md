---
UID: NF:scesvc.ISceSvcAttachmentPersistInfo.Save
title: ISceSvcAttachmentPersistInfo::Save
author: windows-sdk-content
description: The Save method causes the snap-in extension to return information about the data that needs to be saved. The caller is responsible for saving the data.
old-location: security\iscesvcattachmentpersistinfo_save.htm
tech.root: secmgmt
ms.assetid: bdec64b8-2a92-4165-95ff-0de981f2d878
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ISceSvcAttachmentPersistInfo interface [Security],Save method, ISceSvcAttachmentPersistInfo.Save, ISceSvcAttachmentPersistInfo::Save, Save, Save method [Security], Save method [Security],ISceSvcAttachmentPersistInfo interface, _config_iscesvcattachmentpersistinfo_save, scesvc/ISceSvcAttachmentPersistInfo::Save, security.iscesvcattachmentpersistinfo_save
ms.topic: method
req.header: scesvc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Wsecedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wsecedit.dll
api_name:
 - ISceSvcAttachmentPersistInfo.Save
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISceSvcAttachmentPersistInfo::Save


## -description


The <b>Save</b> method causes the snap-in extension to return information about the data that needs to be saved. The caller is responsible for saving the data.


## -parameters




### -param lpTemplateName [in]

Pointer to a null-terminated string that contains the security template name to save data to.


### -param scesvcHandle [in]

Pointer that receives the 
<a href="https://msdn.microsoft.com/478d7d4b-7983-4247-b8be-2e2cd3327533">SCESVC_HANDLE</a> the attachment snap-in extension is using to communicate with the Security Configuration snap-ins.


### -param ppvData [out]

Pointer that receives a buffer that contains the data to be saved.


### -param pbOverwriteAll [out]

Pointer to a <b>BOOL</b> that receives a value indicating whether preexisting data should be overwritten.


## -returns



The return value is an HRESULT. A value of S_OK indicates the method was successful.




## -remarks



The caller should free the buffer set in <i>ppvData</i> by calling 
<a href="https://msdn.microsoft.com/b41f01a4-dc38-4954-a3c5-19fa72910d6f">ISceSvcAttachmentPersistInfo::FreeBuffer</a>.




## -see-also




<a href="https://msdn.microsoft.com/3cd4bde2-55f6-4ab1-b175-7689b0cc529b">ISceSvcAttachmentPersistInfo</a>



<a href="https://msdn.microsoft.com/b41f01a4-dc38-4954-a3c5-19fa72910d6f">ISceSvcAttachmentPersistInfo::FreeBuffer</a>



<a href="https://msdn.microsoft.com/b430e598-e16c-47fc-8f19-fbcfc6b71337">ISceSvcAttachmentPersistInfo::IsDirty</a>



<a href="https://msdn.microsoft.com/478d7d4b-7983-4247-b8be-2e2cd3327533">SCESVC_HANDLE</a>
 

 

