---
UID: NE:certenroll.CommitTemplateFlags
title: CommitTemplateFlags (certenroll.h)
author: windows-sdk-content
description: Specifies options for saving and deleting templates.
old-location: security\committemplateflags.htm
tech.root: seccertenroll
ms.assetid: e228928a-ef11-4caa-b33f-fe25a3a6ff86
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CommitFlagDeleteTemplate, CommitFlagSaveTemplateGenerateOID, CommitFlagSaveTemplateOverwrite, CommitFlagSaveTemplateUseCurrentOID, CommitTemplateFlags, CommitTemplateFlags enumeration [Security], certenroll/CommitFlagDeleteTemplate, certenroll/CommitFlagSaveTemplateGenerateOID, certenroll/CommitFlagSaveTemplateOverwrite, certenroll/CommitFlagSaveTemplateUseCurrentOID, certenroll/CommitTemplateFlags, security.committemplateflags
ms.topic: enum
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - Certenroll.h
api_name:
 - CommitTemplateFlags
product: Windows
targetos: Windows
req.typenames: CommitTemplateFlags
req.redist: 
---

# CommitTemplateFlags enumeration


## -description


The <b>CommitTemplateFlags</b> enumeration type specifies options for saving and deleting templates. It is used by the <a href="https://msdn.microsoft.com/ee7d5640-8d06-4a1a-bce2-f76ee6276207">Commit</a> method on the <a href="https://msdn.microsoft.com/87660b16-06a8-4a71-8669-24521f1399e4">IX509CertificateTemplateWritable</a> interface.


## -enum-fields




### -field CommitFlagSaveTemplateGenerateOID

Save the template and create an object identifier for it.


### -field CommitFlagSaveTemplateUseCurrentOID

Not used.


### -field CommitFlagSaveTemplateOverwrite

Not used.


### -field CommitFlagDeleteTemplate

Delete the template.


## -see-also




<a href="https://msdn.microsoft.com/ee7d5640-8d06-4a1a-bce2-f76ee6276207">Commit</a>



<a href="https://msdn.microsoft.com/87660b16-06a8-4a71-8669-24521f1399e4">IX509CertificateTemplateWritable</a>
 

 

