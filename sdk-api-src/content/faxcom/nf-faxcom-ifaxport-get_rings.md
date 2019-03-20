---
UID: NF:faxcom.IFaxPort.get_Rings
title: IFaxPort::get_Rings (faxcom.h)
author: windows-sdk-content
description: The IFaxPort::get_Rings property represents the number of rings an incoming fax call should wait before the fax port answers the call.
old-location: fax\_mfax_ifaxport_mfax_ifaxport_get_rings_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_3jjn.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxPort interface [Fax Service],Rings property, IFaxPort.Rings, IFaxPort.get_Rings, IFaxPort::Rings, IFaxPort::get_Rings, IFaxPort::put_Rings, Rings property [Fax Service], Rings property [Fax Service],IFaxPort interface, _mfax_ifaxport_get_rings, fax._mfax_ifaxport_get_rings, fax._mfax_ifaxport_mfax_ifaxport_get_rings_cpp, faxcom/IFaxPort::Rings, faxcom/IFaxPort::get_Rings, faxcom/IFaxPort::put_Rings, get_Rings
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
 - IFaxPort.Rings
 - IFaxPort.get_Rings
 - IFaxPort.put_Rings
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxPort::get_Rings


## -description


The <b>IFaxPort::get_Rings</b> property represents the number of rings an incoming fax call should wait before the fax port answers the call. 

This property is read/write.


## -parameters


## -remarks



<div class="alert"><b>Note</b>  Before setting a value for this property, a fax client application can call the <a href="https://msdn.microsoft.com/en-us/library/ms692798(v=VS.85).aspx">IFaxPort::get_CanModify</a> property to ensure that the client has permission to modify configuration information for the specified fax port.</div>
<div> </div>
The fax server ignores the <b>IFaxPort::get_Rings</b> property unless the specified fax port is enabled to receive faxes.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691281(v=VS.85).aspx">IFaxPort</a>



<a href="https://msdn.microsoft.com/en-us/library/ms690893(v=VS.85).aspx">IFaxPorts</a>
 

 

