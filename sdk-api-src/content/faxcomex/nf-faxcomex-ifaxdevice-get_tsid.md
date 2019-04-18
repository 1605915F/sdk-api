---
UID: NF:faxcomex.IFaxDevice.get_TSID
title: IFaxDevice::get_TSID (faxcomex.h)
author: windows-sdk-content
description: The IFaxDevice::get_TSID property is a null-terminated string that contains the transmitting station identifier (TSID) for the device.
old-location: fax\_mfax_faxdevice_cpp_mfax_faxdevice_tsid_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_1c10.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IFaxDevice interface [Fax Service],TSID property, IFaxDevice.TSID, IFaxDevice.get_TSID, IFaxDevice.put_TSID, IFaxDevice::TSID, IFaxDevice::get_TSID, IFaxDevice::put_TSID, TSID property [Fax Service], TSID property [Fax Service],IFaxDevice interface, _mfax_faxdevice.tsid, fax._mfax_faxdevice_cpp_mfax_faxdevice_tsid_cpp, fax._mfax_faxdevice_tsid, faxcomex/IFaxDevice::TSID, faxcomex/IFaxDevice::get_TSID, faxcomex/IFaxDevice::put_TSID, get_TSID
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
 - IFaxDevice.TSID
 - IFaxDevice.get_TSID
 - IFaxDevice.put_TSID
 - IFaxDevice.get_TSID
 - IFaxDevice.put_TSID
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFaxDevice::get_TSID


## -description


The <b>IFaxDevice::get_TSID</b> property is a null-terminated string that contains the transmitting station identifier (TSID) for the device.

This property is read/write.


## -parameters


## -remarks



<div class="alert"><b>Note</b>  The TSID is limited to 20 characters. Also, because most fax machines accept a limited set of characters in the fax transmission called station identifier (CSID) and TSID strings, it is advisable to use only English letters, numeric symbols, and punctuation marks (ASCII range 0x20 to 0x7F) in these strings.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms686192(v=VS.85).aspx">FaxDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/ms686193(v=VS.85).aspx">IFaxDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693400(v=VS.85).aspx">Visual Basic Example</a>
 

 

