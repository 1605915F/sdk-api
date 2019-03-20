---
UID: NS:wmsdkidl.WMDRM_IMPORT_INIT_STRUCT
title: WMDRM_IMPORT_INIT_STRUCT (wmsdkidl.h)
author: windows-sdk-content
description: The WMDRM_IMPORT_INIT_STRUCT structure holds the encrypted session key and content key used in importing protected content.
old-location: wmformat\wmdrm_import_init_struct.htm
tech.root: wmformat
ms.assetid: 191b844e-5760-44d7-9b27-9fa87fead90f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WMDRM_IMPORT_INIT_STRUCT, WMDRM_IMPORT_INIT_STRUCT structure [windows Media Format], structure [windows Media Format], wmformat.wmdrm_import_init_struct, wmsdkidl/WMDRM_IMPORT_INIT_STRUCT
ms.topic: struct
req.header: wmsdkidl.h
req.include-header: Drmexternals.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only],Windows Media Format 11 SDK
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - wmsdkidl.h
api_name:
 - WMDRM_IMPORT_INIT_STRUCT
product: Windows
targetos: Windows
req.typenames: WMDRM_IMPORT_INIT_STRUCT
req.redist: 
---

# WMDRM_IMPORT_INIT_STRUCT structure


## -description



The <b>WMDRM_IMPORT_INIT_STRUCT</b> structure holds the encrypted session key and content key used in importing protected content.




## -struct-fields




### -field dwVersion

Version.


### -field cbEncryptedSessionKeyMessage

Size of the encrypted session key message in bytes.


### -field pbEncryptedSessionKeyMessage

Address of a buffer containing the encrypted session key message. This message is contained in a field of a <a href="https://msdn.microsoft.com/2dd1e8ec-a25f-4ced-8f1b-286534c66ebf">WMDRM_IMPORT_SESSION_KEY</a> structure. The message and its associated key data are both encrypted with the Windows Media DRM machine public key.


### -field cbEncryptedKeyMessage

Size of the encrypted key message in bytes.


### -field pbEncryptedKeyMessage

Address of a buffer containing the encrypted key message. This message is contained in a field of a <a href="https://msdn.microsoft.com/29a0f98d-96a3-46b2-a67c-dbb23449e927">WMDRM_IMPORT_CONTENT_KEY</a> structure. The message and its associated key data are both encrypted with the Windows Media DRM machine public key.


## -remarks



This structure is used to initialize protected stream sample writing in a call to the <a href="https://msdn.microsoft.com/en-us/library/Dd798376(v=VS.85).aspx">IWMDRMWriter3::SetProtectStreamSamples</a> method.




## -see-also




<a href="https://msdn.microsoft.com/118ef278-ca4f-4c30-9633-a2d851f5c758">Structures</a>
 

 

