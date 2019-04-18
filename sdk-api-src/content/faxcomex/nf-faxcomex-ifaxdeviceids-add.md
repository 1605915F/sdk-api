---
UID: NF:faxcomex.IFaxDeviceIds.Add
title: IFaxDeviceIds::Add (faxcomex.h)
author: windows-sdk-content
description: The IFaxDeviceIds::Add method adds a fax device to the FaxDeviceIds collection, using the device's ID.
old-location: fax\_mfax_faxdeviceids_cpp_mfax_faxdeviceids_add_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_4g2s.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Add, Add method [Fax Service], Add method [Fax Service],IFaxDeviceIds interface, IFaxDeviceIds interface [Fax Service],Add method, IFaxDeviceIds.Add, IFaxDeviceIds::Add, _mfax_faxdeviceids.add, fax._mfax_faxdeviceids_add, fax._mfax_faxdeviceids_cpp_mfax_faxdeviceids_add_cpp, faxcomex/IFaxDeviceIds::Add
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
 - IFaxDeviceIds.Add
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFaxDeviceIds::Add


## -description


The <b>IFaxDeviceIds::Add</b> method adds a fax device to the <a href="https://msdn.microsoft.com/en-us/library/ms686501(v=VS.85).aspx">FaxDeviceIds</a> collection, using the device's ID.


## -parameters




### -param lDeviceId [in]

Type: <b>long</b>

A <b>long</b> value that specifies the ID of the fax device to add to the collection.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method can also return remote procedure call (RPC) return values. For more information, see <a href="https://msdn.microsoft.com/en-us/library/Aa378645(v=VS.85).aspx">RPC Return Values</a>.

<div class="alert"><b>Note</b>  You cannot add devices to the special <b>All Devices</b> routing group. Also, you can only add valid device IDs. You can obtain the valid ID of a device in the <a href="https://msdn.microsoft.com/en-us/library/ms686501(v=VS.85).aspx">FaxDeviceIds</a> collection through the <a href="https://msdn.microsoft.com/en-us/library/ms684582(v=VS.85).aspx">Id</a> property.</div>
<div> </div>
To use this method, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farMANAGE_CONFIG</a> access right.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms686501(v=VS.85).aspx">FaxDeviceIds</a>



<a href="https://msdn.microsoft.com/en-us/library/ms686503(v=VS.85).aspx">IFaxDeviceIds</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693408(v=VS.85).aspx">Visual Basic Example</a>
 

 

