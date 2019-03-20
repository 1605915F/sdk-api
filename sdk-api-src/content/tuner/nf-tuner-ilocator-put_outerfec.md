---
UID: NF:tuner.ILocator.put_OuterFEC
title: ILocator::put_OuterFEC (tuner.h)
author: windows-sdk-content
description: The put_OuterFEC method sets the type of outer FEC to use.
old-location: mstv\ilocator_put_outerfec.htm
tech.root: mstv
ms.assetid: 0aaa4d8e-e760-4e22-90fe-e5667fafa113
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDigitalLocatorput_OuterFEC, ILocator interface [Microsoft TV Technologies],put_OuterFEC method, ILocator.put_OuterFEC, ILocator::put_OuterFEC, mstv.ilocator_put_outerfec, put_OuterFEC, put_OuterFEC method [Microsoft TV Technologies], put_OuterFEC method [Microsoft TV Technologies],ILocator interface, tuner/ILocator::put_OuterFEC
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
 - ILocator.put_OuterFEC
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ILocator::put_OuterFEC


## -description



The <b>put_OuterFEC</b> method sets the type of outer FEC to use.




## -parameters




### -param FEC [in]

Specifies the outer FEC. This parameter is a value of type <a href="https://msdn.microsoft.com/6910c51d-4176-49a3-be6b-6b072ad03fc1">FECMethod</a>.


## -returns



Returns S_OK if successful. If the method fails, error information can be retrieved using the standard COM <b>IErrorInfo</b> interface.




## -see-also




<a href="https://msdn.microsoft.com/1d6c18f0-e7f1-4a1c-9edb-e4b66297becf">ILocator</a>



<a href="https://msdn.microsoft.com/library/Dd693582(v=VS.85).aspx">get_OuterFEC</a>



<a href="https://msdn.microsoft.com/library/Dd693585(v=VS.85).aspx">put_InnerFEC</a>



<a href="https://msdn.microsoft.com/library/Dd693588(v=VS.85).aspx">put_OuterFECRate</a>
 

 

