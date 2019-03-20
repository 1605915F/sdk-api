---
UID: NF:faxcomex.IFaxDeviceIds.get_Item
title: IFaxDeviceIds::get_Item (faxcomex.h)
author: windows-sdk-content
description: The IFaxDeviceIds::get_Item method represents a device ID from the FaxDeviceIds collection.
old-location: fax\_mfax_faxdeviceids_item_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_0xt9_cpp.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxDeviceIds interface [Fax Service],get_Item method, IFaxDeviceIds.get_Item, IFaxDeviceIds::get_Item, _mfax_faxdeviceids.item_cpp, fax._mfax_faxdeviceids_item_cpp, faxcomex/IFaxDeviceIds::get_Item, get_Item, get_Item method [Fax Service], get_Item method [Fax Service],IFaxDeviceIds interface
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
 - IFaxDeviceIds.get_Item
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxDeviceIds::get_Item


## -description


The <b>IFaxDeviceIds::get_Item</b> method represents a device ID from the <a href="https://msdn.microsoft.com/en-us/library/ms686501(v=VS.85).aspx">FaxDeviceIds</a> collection.


## -parameters




### -param lIndex [in]

Type: <b>long</b>

A value specifying the item to retrieve from the collection. Valid values for this parameter are in the range from 1 to n, where n is the number of devices returned by a call to the <a href="https://msdn.microsoft.com/en-us/library/ms686492(v=VS.85).aspx">IFaxDeviceIds::get_Count</a> method.


### -param plDeviceId [out, retval]

Type: <b>long*</b>

Pointer to a value that receives the item requested.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms686501(v=VS.85).aspx">FaxDeviceIds</a>



<a href="https://msdn.microsoft.com/en-us/library/ms686503(v=VS.85).aspx">IFaxDeviceIds</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693408(v=VS.85).aspx">Visual Basic Example</a>
 

 

