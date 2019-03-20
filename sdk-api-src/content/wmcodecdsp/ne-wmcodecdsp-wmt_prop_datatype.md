---
UID: NE:wmcodecdsp.WMT_PROP_DATATYPE
title: WMT_PROP_DATATYPE (wmcodecdsp.h)
author: windows-sdk-content
description: Defines the data types used for the codec and DSP properties that are accessed by using the methods of the IWMCodecProps interface.
old-location: mf\wmt_prop_datatypeenumeration.htm
tech.root: medfound
ms.assetid: 3d7b2ab9-5e5a-4bc7-9d56-c17b838ded67
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WMT_PROP_DATATYPE, WMT_PROP_DATATYPE enumeration [Media Foundation], WMT_PROP_TYPE_BINARY, WMT_PROP_TYPE_BOOL, WMT_PROP_TYPE_DWORD, WMT_PROP_TYPE_GUID, WMT_PROP_TYPE_QWORD, WMT_PROP_TYPE_STRING, WMT_PROP_TYPE_WORD, codecapi.wmt_prop_datatypeenumeration, mf.wmt_prop_datatype, mf.wmt_prop_datatypeenumeration, wmcodecdsp/WMT_PROP_DATATYPE, wmcodecdsp/WMT_PROP_TYPE_BINARY, wmcodecdsp/WMT_PROP_TYPE_BOOL, wmcodecdsp/WMT_PROP_TYPE_DWORD, wmcodecdsp/WMT_PROP_TYPE_GUID, wmcodecdsp/WMT_PROP_TYPE_QWORD, wmcodecdsp/WMT_PROP_TYPE_STRING, wmcodecdsp/WMT_PROP_TYPE_WORD
ms.topic: enum
req.header: wmcodecdsp.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - wmcodecdsp.h
api_name:
 - WMT_PROP_DATATYPE
product: Windows
targetos: Windows
req.typenames: WMT_PROP_DATATYPE
req.redist: 
---

# WMT_PROP_DATATYPE enumeration


## -description


Defines the data types used for the codec and DSP properties that are accessed by using the methods of the <a href="https://msdn.microsoft.com/b49e506b-8c87-44b9-be6c-b9a33f6c9ecb">IWMCodecProps</a> interface.




## -enum-fields




### -field WMT_PROP_TYPE_DWORD

Specifies a double-word value.


### -field WMT_PROP_TYPE_STRING

Specifies a string value.


### -field WMT_PROP_TYPE_BINARY

Specifies a binary value.


### -field WMT_PROP_TYPE_BOOL

Specifies a Boolean value.


### -field WMT_PROP_TYPE_QWORD

Specifies a quadruple-word value.


### -field WMT_PROP_TYPE_WORD

Specifies a word value.


### -field WMT_PROP_TYPE_GUID

Specifies a GUID value.


## -remarks



Most properties are accessed by using the methods of the <b>IPropertyBag</b> interface. The data types of those properties are defined as constants used with <b>VARIANTARG</b> values.






## -see-also




<a href="https://msdn.microsoft.com/f26a730f-18c4-4247-acaf-af1dfad19086">Media Foundation Enumerations</a>
 

 

