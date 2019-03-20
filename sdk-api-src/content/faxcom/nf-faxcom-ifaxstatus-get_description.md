---
UID: NF:faxcom.IFaxStatus.get_Description
title: IFaxStatus::get_Description (faxcom.h)
author: windows-sdk-content
description: Retrieves the Description property for the FaxStatus object of a parent FaxPort object. The Description property is a null-terminated string that describes the current status of the specified port.
old-location: fax\_mfax_ifaxstatus_mfax_ifaxstatus_get_description_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_5goe.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Description property [Fax Service], Description property [Fax Service],IFaxStatus interface, IFaxStatus interface [Fax Service],Description property, IFaxStatus.Description, IFaxStatus.get_Description, IFaxStatus::Description, IFaxStatus::get_Description, _mfax_ifaxstatus_get_description, fax._mfax_ifaxstatus_get_description, fax._mfax_ifaxstatus_mfax_ifaxstatus_get_description_cpp, faxcom/IFaxStatus::Description, faxcom/IFaxStatus::get_Description, get_Description
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
 - IFaxStatus.Description
 - IFaxStatus.get_Description
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxStatus::get_Description


## -description


Retrieves the <b>Description</b> property for the <a href="https://msdn.microsoft.com/en-us/library/ms691355(v=VS.85).aspx">FaxStatus</a> object of a parent <a href="https://msdn.microsoft.com/en-us/library/ms691338(v=VS.85).aspx">FaxPort</a> object. The <b>Description</b> property is a null-terminated string that describes the current status of the specified port.

This property is read-only.


## -parameters


## -remarks



If the descriptive information is not available, the <b>IFaxStatus::get_Description</b> method returns an empty string.

The <b>IFaxStatus::get_Description</b> method allocates the memory required for the buffer pointed to by the <i>pVal</i> parameter. The client application must call the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function to deallocate the resources associated with this parameter. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms690878(v=VS.85).aspx">Freeing Fax Resources</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691281(v=VS.85).aspx">IFaxPort</a>



<a href="https://msdn.microsoft.com/en-us/library/ms690893(v=VS.85).aspx">IFaxPorts</a>



<a href="https://msdn.microsoft.com/en-us/library/ms690794(v=VS.85).aspx">IFaxStatus</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a>
 

 

