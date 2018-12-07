---
UID: NF:faxcomex.IFaxOutgoingJob.CopyTiff
title: IFaxOutgoingJob::CopyTiff
author: windows-sdk-content
description: The IFaxOutgoingJob::CopyTiff method copies the Tagged Image File Format Class F (TIFF Class F) file associated with the outbound fax job, to a file on the local computer.
old-location: fax\_mfax_faxoutgoingjob_cpp_mfax_faxoutgoingjob_copytiff_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_8mli.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CopyTiff, CopyTiff method [Fax Service], CopyTiff method [Fax Service],IFaxOutgoingJob interface, IFaxOutgoingJob interface [Fax Service],CopyTiff method, IFaxOutgoingJob.CopyTiff, IFaxOutgoingJob::CopyTiff, _mfax_faxoutgoingjob.copytiff, fax._mfax_faxoutgoingjob_copytiff, fax._mfax_faxoutgoingjob_cpp_mfax_faxoutgoingjob_copytiff_cpp, faxcomex/IFaxOutgoingJob::CopyTiff
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxOutgoingJob.CopyTiff
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutgoingJob::CopyTiff


## -description


The <b>IFaxOutgoingJob::CopyTiff</b> method copies the Tagged Image File Format Class F (TIFF Class F) file associated with the outbound fax job, to a file on the local computer.


## -parameters




### -param bstrTiffPath

Type: <b>BSTR</b>

Null-terminated string that contains a fully qualified path and file name on the local computer. The fax service will copy the TIFF Class F file associated with the outbound fax to the specified file.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To use this method, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farSUBMIT_LOW</a> or <b>farQUERY_JOBS</b> access right.

With the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farSUBMIT_LOW</a> access right, users will be able to use this method only for their own faxes. With the <b>farQUERY_JOBS</b> access right, users will be able to use this method for all faxes on the server.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms689115(v=VS.85).aspx">FaxOutgoingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms689116(v=VS.85).aspx">IFaxOutgoingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693393(v=VS.85).aspx">Visual Basic Example</a>
 

 

