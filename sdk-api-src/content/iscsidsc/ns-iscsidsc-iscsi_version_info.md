---
UID: NS:iscsidsc.__unnamed_struct_24
title: ISCSI_VERSION_INFO (iscsidsc.h)
author: windows-sdk-content
description: The ISCSI_VERSION_INFO structure contains the version and build numbers of the iSCSI software initiator and the initiator service.
old-location: iscsidisc\iscsi_version_info.htm
tech.root: iSCSIDisc
ms.assetid: 04b9e0c0-2c1e-4553-8eef-697819075bc4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PISCSI_VERSION_INFO, ISCSI_VERSION_INFO, ISCSI_VERSION_INFO structure [iSCSI Discovery Library API], PISCSI_VERSION_INFO, PISCSI_VERSION_INFO structure pointer [iSCSI Discovery Library API], iscsidisc.iscsi_version_info, iscsidsc/ISCSI_VERSION_INFO, iscsidsc/PISCSI_VERSION_INFO"
ms.topic: struct
req.header: iscsidsc.h
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
 - Iscsidsc.h
api_name:
 - ISCSI_VERSION_INFO
product: Windows
targetos: Windows
req.typenames: ISCSI_VERSION_INFO, *PISCSI_VERSION_INFO
req.redist: 
---

# ISCSI_VERSION_INFO structure


## -description


The <b>ISCSI_VERSION_INFO</b> structure contains the version and build numbers of the iSCSI software initiator and the initiator service.



## -struct-fields




### -field MajorVersion

The major version number of the iSCSI software initiator and initiator service. This may be different from the version number of the Operating System. 


### -field MinorVersion

The minor version number of the iSCSI software initiator and initiator service. This may be different from the version number of the Operating System.


### -field BuildNumber

The build number of the iSCSI software initiator and initiator service. This may be different from the build number of the Operating System. 

