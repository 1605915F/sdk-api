---
UID: NF:mswmdm.IWMDMStorage2.GetAttributes2
title: IWMDMStorage2::GetAttributes2 (mswmdm.h)
author: windows-sdk-content
description: The GetAttributes2 method retrieves extended attributes of the storage.
old-location: wmdm\iwmdmstorage2_getattributes2.htm
tech.root: WMDM
ms.assetid: 8212ab78-0a2a-41cd-8a7c-da6e3886b586
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetAttributes2, GetAttributes2 method [windows Media Device Manager], GetAttributes2 method [windows Media Device Manager],IWMDMStorage2 interface, IWMDMStorage2 interface [windows Media Device Manager],GetAttributes2 method, IWMDMStorage2.GetAttributes2, IWMDMStorage2::GetAttributes2, IWMDMStorage2GetAttributes2, mswmdm/IWMDMStorage2::GetAttributes2, wmdm.iwmdmstorage2_getattributes2
ms.topic: method
req.header: mswmdm.h
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
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mssachlp.lib
 - mssachlp.dll
api_name:
 - IWMDMStorage2.GetAttributes2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMStorage2::GetAttributes2


## -description



The <b>GetAttributes2</b> method retrieves extended attributes of the storage.




## -parameters




### -param pdwAttributes [out]

Pointer to a <b>DWORD</b> specifying one or more attributes defined in the <a href="https://msdn.microsoft.com/e43139d2-260a-4f27-a06c-aca741204663">IWMDMStorage::GetAttributes</a> method, combined with a bitwise <b>OR</b>.


### -param pdwAttributesEx [out]

Pointer to a <b>DWORD</b> specifying the extended attributes. Currently, no extended attributes are defined.


### -param pAudioFormat [out]

Optional pointer to a <a href="https://msdn.microsoft.com/2128f07a-4858-49b7-b031-16d4a84c9d32">_ WAVEFORMATEX</a> structure that specifies audio information about the object. This parameter is ignored if the file is not audio.


### -param pVideoFormat [out]

Optional pointer to a <a href="https://msdn.microsoft.com/5a39d66e-8dbc-4572-8370-14f722b6c906">_ VIDEOINFOHEADER</a> structure that specifies video information about the object. This parameter is ignored if the file is not video.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -remarks



Evaluation of attributes is a crucial step when exposing the contents of the media device. Some devices do not support hierarchical storage of data on storage media. The <b>GetAttributes2</b> method is used to infer the support and format of the file system by discovering its structure through object attributes.




## -see-also




<a href="https://msdn.microsoft.com/6ea80ab2-718b-464e-a805-9910460931bb">IWMDMEnumStorage Interface</a>



<a href="https://msdn.microsoft.com/1283a5b5-d893-4795-a50a-5a3bd6fce8d5">IWMDMStorage2 Interface</a>



<a href="https://msdn.microsoft.com/0a2e143e-8d6a-497e-9c45-fd3349c4ec97">IWMDMStorage2::SetAttributes2</a>



<a href="https://msdn.microsoft.com/ab3c6a17-5a86-419b-b528-fd0db718de8f">IWMDMStorage::EnumStorage</a>
 

 

