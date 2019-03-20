---
UID: NF:tuner.IPersistTuneXmlUtility.Deserialize
title: IPersistTuneXmlUtility::Deserialize (tuner.h)
author: windows-sdk-content
description: Constructs and returns an object that initializes itself by using the XML node passed as a VARIANT parameter to the method. The returned object exposes its IUnknown interface so that other objects can query it.
old-location: mstv\ipersisttunexmlutility_deserialize.htm
tech.root: mstv
ms.assetid: a42a001b-210c-4e89-823e-ec1e1fa58f67
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Deserialize, Deserialize method [Microsoft TV Technologies], Deserialize method [Microsoft TV Technologies],IPersistTuneXmlUtility interface, IPersistTuneXmlUtility interface [Microsoft TV Technologies],Deserialize method, IPersistTuneXmlUtility.Deserialize, IPersistTuneXmlUtility::Deserialize, mstv.ipersisttunexmlutility_deserialize, tuner/IPersistTuneXmlUtility::Deserialize
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
 - tuner.h
api_name:
 - IPersistTuneXmlUtility.Deserialize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPersistTuneXmlUtility::Deserialize


## -description


Constructs and returns an object that initializes itself by using the XML node passed as a <b>VARIANT</b> parameter to the method. The returned object exposes its <b>IUnknown</b> interface so that other objects can query it.


## -parameters




### -param varValue [in]

XML node used to construct and initialize the object. This parameter can be either a <b>BSTR</b> object or an <b>IXMLDOMNode</b> object.
          


### -param ppObject [out, retval]

Pointer to the <b>IUnknown</b> interface of the object being deserialized.
          This method allocates memory to hold the deserialized object and returns the pointer in this parameter. The caller is responsible for freeing this memory.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/aa03015f-094f-499f-99fb-2e15ead74f15">IPersistTuneXmlUtility</a>
 

 

