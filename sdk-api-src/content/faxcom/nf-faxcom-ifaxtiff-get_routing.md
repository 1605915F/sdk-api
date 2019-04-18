---
UID: NF:faxcom.IFaxTiff.get_Routing
title: IFaxTiff::get_Routing (faxcom.h)
author: windows-sdk-content
description: Retrieves the Routing property for a FaxTiff object. The Routing property is a null-terminated string that contains the inbound routing string for a specified fax file.
old-location: fax\_mfax_ifaxtiff_mfax_ifaxtiff_get_routing_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_39lz.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IFaxTiff interface [Fax Service],Routing property, IFaxTiff.Routing, IFaxTiff.get_Routing, IFaxTiff::Routing, IFaxTiff::get_Routing, Routing property [Fax Service], Routing property [Fax Service],IFaxTiff interface, _mfax_ifaxtiff_get_routing, fax._mfax_ifaxtiff_get_routing, fax._mfax_ifaxtiff_mfax_ifaxtiff_get_routing_cpp, faxcom/IFaxTiff::Routing, faxcom/IFaxTiff::get_Routing, get_Routing
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
 - IFaxTiff.Routing
 - IFaxTiff.get_Routing
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFaxTiff::get_Routing


## -description


Retrieves the <b>Routing</b> property for a <a href="https://msdn.microsoft.com/en-us/library/ms691832(v=VS.85).aspx">FaxTiff</a> object. The <b>Routing</b> property is a null-terminated string that contains the inbound routing string for a specified fax file.

This property is read-only.


## -parameters


## -remarks



A fax client application must  set the <a href="https://msdn.microsoft.com/en-us/library/ms690773(v=VS.85).aspx">Image</a> property before retrieving another property for a <a href="https://msdn.microsoft.com/en-us/library/ms691832(v=VS.85).aspx">FaxTiff</a> object.

The routing information is specific to a fax service provider (FSP); for example, direct inward dialing (DID) routing digits.

The <b>get_Routing</b> method sets the <i>pVal</i> parameter to optional inbound routing information specified for the fax file, if it is available. If the information is not available, the method returns "Unavailable".

The <b>Routing</b> property is a string that represents optional inbound routing information specified for the fax file, if it is available. If the information is not available, <b>Routing</b> is an empty string.

The <a href="https://msdn.microsoft.com/en-us/library/ms690773(v=VS.85).aspx">get_Image</a> method allocates the memory required for the buffer pointed to by the <i>pVal</i> parameter. The client application must call the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function to deallocate the resources associated with this parameter. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms690878(v=VS.85).aspx">Freeing Fax Resources</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691802(v=VS.85).aspx">IFaxTiff</a>



<a href="https://msdn.microsoft.com/en-us/library/ms690773(v=VS.85).aspx">IFaxTiff::get_Image</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a>
 

 

