---
UID: NF:d3d12.ID3D12Object.SetPrivateDataInterface
title: ID3D12Object::SetPrivateDataInterface
author: windows-sdk-content
description: Associates an IUnknown-derived interface with the device object and associates that interface with an application-defined GUID.
old-location: direct3d12\id3d12object_setprivatedatainterface.htm
tech.root: direct3d12
ms.assetid: B03B9420-7E85-4C1A-858C-37B20E4D9B52
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D12Object interface,SetPrivateDataInterface method, ID3D12Object.SetPrivateDataInterface, ID3D12Object::SetPrivateDataInterface, SetPrivateDataInterface, SetPrivateDataInterface method, SetPrivateDataInterface method,ID3D12Object interface, d3d12/ID3D12Object::SetPrivateDataInterface, direct3d12.id3d12object_setprivatedatainterface
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d12.h
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
req.lib: D3D12.lib
req.dll: D3D12.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D12.dll
api_name:
 - ID3D12Object.SetPrivateDataInterface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12Object::SetPrivateDataInterface


## -description


Associates an <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a>-derived interface with the device object and associates that interface with an application-defined <b>GUID</b>.
        


## -parameters




### -param guid [in]

Type: <b><a href="http://msdn.microsoft.com/en-us/library/cc237815(PROT.13).aspx">REFGUID</a></b>

The <b>GUID</b> to associate with the interface.
          


### -param pData [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a>*</b>

A pointer to the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a>-derived interface to be associated with the device object.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/en-us/library/Dn706075(v=VS.85).aspx">Direct3D 12 Return Codes</a>.
          




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn788699(v=VS.85).aspx">ID3D12Object</a>
 

 

