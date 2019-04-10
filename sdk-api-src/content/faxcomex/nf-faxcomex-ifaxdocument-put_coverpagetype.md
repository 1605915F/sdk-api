---
UID: NF:faxcomex.IFaxDocument.put_CoverPageType
title: IFaxDocument::put_CoverPageType (faxcomex.h)
author: windows-sdk-content
description: The IFaxDocument::get_CoverPageType property is a value from an enumeration that indicates whether a specified cover page template file (.cov) is a server-based cover page file or a local-computer-based cover page file.
old-location: fax\_mfax_faxdocument_cpp_mfax_faxdocument_coverpagetype_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_3v8l.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CoverPageType property [Fax Service], CoverPageType property [Fax Service],IFaxDocument interface, IFaxDocument interface [Fax Service],CoverPageType property, IFaxDocument.CoverPageType, IFaxDocument.put_CoverPageType, IFaxDocument::CoverPageType, IFaxDocument::get_CoverPageType, IFaxDocument::put_CoverPageType, _mfax_faxdocument.coverpagetype, fax._mfax_faxdocument_coverpagetype, fax._mfax_faxdocument_cpp_mfax_faxdocument_coverpagetype_cpp, faxcomex/IFaxDocument::CoverPageType, faxcomex/IFaxDocument::get_CoverPageType, faxcomex/IFaxDocument::put_CoverPageType, put_CoverPageType
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
 - IFaxDocument.CoverPageType
 - IFaxDocument.get_CoverPageType
 - IFaxDocument.put_CoverPageType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxDocument::put_CoverPageType


## -description


The <b>IFaxDocument::get_CoverPageType</b> property is a value from an enumeration that indicates whether a specified cover page template file (.cov) is a server-based cover page file or a local-computer-based cover page file. You can also specify that no file is used.

This property is read/write.


## -parameters


## -remarks



By default, <b>IFaxDocument::get_CoverPageType</b> is set to <a href="https://msdn.microsoft.com/en-us/library/ms689603(v=VS.85).aspx">fcptNONE</a>, indicating that no file is used.

Provide the name of the cover page in the <a href="https://msdn.microsoft.com/en-us/library/ms687493(v=VS.85).aspx">IFaxDocument::get_CoverPage</a> property.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms685958(v=VS.85).aspx">FaxDocument</a>



<a href="https://msdn.microsoft.com/en-us/library/ms685960(v=VS.85).aspx">IFaxDocument</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692936(v=VS.85).aspx">Visual Basic Example</a>
 

 

