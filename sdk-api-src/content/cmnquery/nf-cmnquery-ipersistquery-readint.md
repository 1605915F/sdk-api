---
UID: NF:cmnquery.IPersistQuery.ReadInt
title: IPersistQuery::ReadInt
author: windows-sdk-content
description: Reads an integer value from the query store.
old-location: ad\ipersistquery_readint.htm
tech.root: ad
ms.assetid: e7db105f-d331-4048-8d75-e85af94a5c54
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPersistQuery interface [Active Directory],ReadInt method, IPersistQuery.ReadInt, IPersistQuery::ReadInt, ReadInt, ReadInt method [Active Directory], ReadInt method [Active Directory],IPersistQuery interface, _glines_ipersistquery_readint, ad.ipersistquery__readint, ad.ipersistquery_readint, cmnquery/IPersistQuery::ReadInt
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: cmnquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Dsquery.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dsquery.dll
api_name:
 - IPersistQuery.ReadInt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPersistQuery::ReadInt


## -description


The <b>IPersistQuery::ReadInt</b> method reads an integer value from the query  store.


## -parameters




### -param pSection [in]

A pointer to a null-terminated Unicode string that represents the section name that the integer should be read from.


### -param pValueName [in]

A pointer to a null-terminated Unicode string that represents the name of the integer value to be read.


### -param pValue [out]

Pointer to an integer variable that receives the integer value.


## -returns



Returns <b>S_OK</b> if successful or a standard  <b>HRESULT</b> value otherwise. Possible error codes include the following.




## -see-also




<a href="https://msdn.microsoft.com/f53d4425-5496-45f8-a09b-f163b63a29c8">Display Interfaces in Active Directory Domain Services</a>



<a href="https://msdn.microsoft.com/9d90f119-3d10-4f06-bed4-5ffab9ae14a4">IPersistQuery</a>
 

 

