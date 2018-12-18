---
UID: NF:casetup.IMSCEPSetup.GetKeyLengthList
title: IMSCEPSetup::GetKeyLengthList
author: windows-sdk-content
description: Gets the list of key lengths supported by the specified cryptographic service provider (CSP).
old-location: security\imscepsetup_getkeylengthlist.htm
tech.root: seccrypto
ms.assetid: 992619dd-1d59-4033-b3aa-ae32dc9948c2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetKeyLengthList, GetKeyLengthList method [Security], GetKeyLengthList method [Security],IMSCEPSetup interface, IMSCEPSetup interface [Security],GetKeyLengthList method, IMSCEPSetup.GetKeyLengthList, IMSCEPSetup::GetKeyLengthList, casetup/IMSCEPSetup::GetKeyLengthList, security.imscepsetup_getkeylengthlist
ms.topic: method
req.header: casetup.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Casetup.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Certocm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certocm.dll
api_name:
 - IMSCEPSetup.GetKeyLengthList
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSCEPSetup::GetKeyLengthList


## -description


The <b>GetKeyLengthList</b> method gets the list of <a href="https://msdn.microsoft.com/f17042c3-ba1a-408f-af55-5f171b0dee33">key lengths</a> supported by the specified <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">cryptographic service provider</a> (CSP).


## -parameters




### -param bExchange [in]

A value that indicates whether the listed lengths are for an exchange key algorithm. A <b>VARIANT_TRUE</b>  value indicates exchange key lengths; otherwise, the lengths are for signing keys.


### -param bstrProviderName [in]

A string that contains the name of the CSP.


### -param pVal [out]

A pointer to a  <b>VARIANT</b> array of <b>VT_UI4</b> types that correspond to the key lengths supported by the CSP.


## -see-also




<a href="https://msdn.microsoft.com/328c6c04-7ade-4b64-bd8a-4314b6e8dc78">IMSCEPSetup</a>
 

 

