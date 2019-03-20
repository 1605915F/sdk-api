---
UID: NF:faxcom.IFaxTiff.get_Tsid
title: IFaxTiff::get_Tsid (faxcom.h)
author: windows-sdk-content
description: Retrieves the Tsid property for a FaxTiff object. The Tsid property is a null-terminated string that contains transmitting station identifier (TSID) information, which is typically the fax number of the device that sent the specified fax file.
old-location: fax\_mfax_ifaxtiff_mfax_ifaxtiff_get_tsid_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_7tes.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxTiff interface [Fax Service],Tsid property, IFaxTiff.Tsid, IFaxTiff.get_Tsid, IFaxTiff::Tsid, IFaxTiff::get_Tsid, Tsid property [Fax Service], Tsid property [Fax Service],IFaxTiff interface, _mfax_ifaxtiff_get_tsid, fax._mfax_ifaxtiff_get_tsid, fax._mfax_ifaxtiff_mfax_ifaxtiff_get_tsid_cpp, faxcom/IFaxTiff::Tsid, faxcom/IFaxTiff::get_Tsid, get_Tsid
ms.topic: method
req.header: faxcom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
req.dll: Faxcom.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Faxcom.dll
api_name:
 - IFaxTiff.Tsid
 - IFaxTiff.get_Tsid
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxTiff::get_Tsid


## -description


Retrieves the <b>Tsid</b> property for a <a href="https://msdn.microsoft.com/en-us/library/ms691832(v=VS.85).aspx">FaxTiff</a> object. The <b>Tsid</b> property is a null-terminated string that contains transmitting station identifier (TSID) information, which is typically the fax number of the device that sent the specified fax file.

This property is read-only.


## -parameters


## -remarks



A fax client application must  set the <a href="https://msdn.microsoft.com/en-us/library/ms690773(v=VS.85).aspx">Image</a> property before retrieving another property for a <a href="https://msdn.microsoft.com/en-us/library/ms691832(v=VS.85).aspx">FaxTiff</a> object.

The <b>get_Tsid</b> method sets the <i>pVal</i> parameter to the TSID associated with the specified fax file, if it is available. If the information is not available, the method returns "Unavailable".

The <b>Tsid</b> property is a string that represents the TSID associated with the specified fax file, if it is available. If the information is not available, <b>Tsid</b> is an empty string.

The <b>get_Tsid</b> method allocates the memory required for the buffer pointed to by the <i>pVal</i> parameter. The client application must call the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function to deallocate the resources associated with this parameter. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms690878(v=VS.85).aspx">Freeing Fax Resources</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691802(v=VS.85).aspx">IFaxTiff</a>



<a href="https://msdn.microsoft.com/en-us/library/ms690773(v=VS.85).aspx">IFaxTiff::get_Image</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a>
 

 

