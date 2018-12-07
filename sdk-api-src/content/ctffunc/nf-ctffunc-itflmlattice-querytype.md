---
UID: NF:ctffunc.ITfLMLattice.QueryType
title: ITfLMLattice::QueryType
author: windows-sdk-content
description: ITfLMLattice::QueryType method
old-location: tsf\itflmlattice_querytype.htm
tech.root: TSF
ms.assetid: 199032f7-b97f-4475-9ce3-9af952e13f12
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITfLMLattice interface [Text Services Framework],QueryType method, ITfLMLattice.QueryType, ITfLMLattice::QueryType, QueryType, QueryType method [Text Services Framework], QueryType method [Text Services Framework],ITfLMLattice interface, _tsf_itflmlattice_querytype_ref, ctffunc/ITfLMLattice::QueryType, tsf.itflmlattice_querytype
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: ctffunc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Ctffunc.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msctf.dll
api_name:
 - ITfLMLattice.QueryType
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfLMLattice::QueryType


## -description




## -parameters




### -param rguidType [in]

Specifies the lattice type identifier. This can be one of the <a href="https://msdn.microsoft.com/en-us/library/ms628996(v=VS.85).aspx">Lattice Type</a> values.


### -param pfSupported [out]

Pointer to a <b>BOOL</b> that receives a value that indicates if the lattice type is supported. If the lattice type is supported, this parameter receives a nonzero value and the method returns S_OK. If the lattice type is unsupported, this parameter receives zero and the method returns E_INVALIDARG.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The specified lattice type is supported.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Either <i>pfSupported</i> is invalid or the specified lattice type is not supported.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms628774(v=VS.85).aspx">ITfLMLattice</a>



<a href="https://msdn.microsoft.com/ce4bf11b-e7e7-4f06-b572-8ed6f0ed8d36">Lattice Types
      </a>
 

 

