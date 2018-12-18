---
UID: NS:oaidl.tagVARDESC
title: VARDESC
author: windows-sdk-content
description: Describes a variable, constant, or data member.
old-location: automat\vardesc.htm
tech.root: automat
ms.assetid: 9584977d-41c4-4f73-8844-2135750ddb80
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPVARDESC, LPVARDESC, LPVARDESC structure pointer [Automation], VARDESC, VARDESC structure [Automation], _oa96_VARDESC, automat.vardesc, oaidl/LPVARDESC, oaidl/VARDESC"
ms.topic: struct
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - OaIdl.h
api_name:
 - VARDESC
product: Windows
targetos: Windows
req.typenames: VARDESC, *LPVARDESC
req.redist: 
---

# VARDESC structure


## -description


Describes a variable, constant, or data member.


## -struct-fields




### -field memid

The member ID.


### -field lpstrSchema

Reserved.


### -field DUMMYUNIONNAME

 


### -field DUMMYUNIONNAME.oInst

With VAR_PERINSTANCE, the offset of this variable within the instance.


### -field DUMMYUNIONNAME.lpvarValue

With VAR_CONST, the value of the constant.


### -field elemdescVar

The variable type.


### -field wVarFlags

The variable flags. See <a href="https://msdn.microsoft.com/9422f2a5-d8c0-4d65-ad7a-9eaa9bbedf91">VARFLAGS</a>.


### -field varkind

The variable type.

