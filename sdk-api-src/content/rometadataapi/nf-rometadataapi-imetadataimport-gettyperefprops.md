---
UID: NF:rometadataapi.IMetaDataImport.GetTypeRefProps
title: IMetaDataImport::GetTypeRefProps (rometadataapi.h)
author: windows-sdk-content
description: Gets the metadata associated with the Type referenced by the specified TypeRef token.
old-location: winrt\imetadataimport_gettyperefprops.htm
tech.root: WinRT
ms.assetid: 714d1adf-df8d-4f6b-8bcd-8dd9461c102a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetTypeRefProps, GetTypeRefProps method [Windows Runtime], GetTypeRefProps method [Windows Runtime],IMetaDataImport interface, IMetaDataImport interface [Windows Runtime],GetTypeRefProps method, IMetaDataImport.GetTypeRefProps, IMetaDataImport::GetTypeRefProps, rometadataapi/IMetaDataImport::GetTypeRefProps, winrt.imetadataimport_gettyperefprops
ms.topic: method
req.header: rometadataapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Rometadataapi.idl
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
 - rometadataapi.h
api_name:
 - IMetaDataImport.GetTypeRefProps
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMetaDataImport::GetTypeRefProps


## -description


Gets the metadata associated with the Type referenced by the specified TypeRef token.


## -parameters




### -param tkTypeRef [in]

The TypeRef token that represents the type to return metadata for.


### -param ptkResolutionScope [out]

A pointer to the scope in which the reference is made. This value is an AssemblyRef or ModuleRef token.


### -param szName [out]

A buffer containing the type name.


### -param cchName [in]

The requested size in wide characters of <i>szName</i>.


### -param pchName [out]

The returned size in wide characters of <i>szName</i>.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/5457d9d3-9a43-4e89-a52f-1254662ed92a">IMetaDataImport</a>
 

 

