---
UID: NF:wmp.IWMPCdromCollection.getByDriveSpecifier
title: IWMPCdromCollection::getByDriveSpecifier
author: windows-sdk-content
description: The getByDriveSpecifier method retrieves a pointer to an IWMPCdrom interface associated with a particular drive letter.
old-location: wmp\iwmpcdromcollection_getbydrivespecifier.htm
tech.root: WMP
ms.assetid: b48679da-c8f3-4e9d-89cd-0ecbcbc07fe4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPCdromCollection interface [Windows Media Player],getByDriveSpecifier method, IWMPCdromCollection.getByDriveSpecifier, IWMPCdromCollection::getByDriveSpecifier, IWMPCdromCollectiongetByDriveSpecifier, getByDriveSpecifier, getByDriveSpecifier method [Windows Media Player], getByDriveSpecifier method [Windows Media Player],IWMPCdromCollection interface, wmp.iwmpcdromcollection_getbydrivespecifier, wmp/IWMPCdromCollection::getByDriveSpecifier
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 9 Series or later.
req.target-min-winversvr: 
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
req.dll: Wmp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmp.dll
api_name:
 - IWMPCdromCollection.getByDriveSpecifier
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPCdromCollection::getByDriveSpecifier


## -description



The <b>getByDriveSpecifier</b> method retrieves a pointer to an <b>IWMPCdrom</b> interface associated with a particular drive letter.




## -parameters




### -param bstrDriveSpecifier [in]

<b>BSTR</b> containing the drive letter followed by a colon (":") character.


### -param ppCdrom [out]

Pointer to a pointer to an <b>IWMPCdrom</b> interface.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



Drive letters must be given in the form <i>X</i>:, where <i>X</i> represents the drive letter.

To use this method, read access to the library is required. For more information, see <a href="https://msdn.microsoft.com/9f722531-a551-4ca9-be5f-01a291a180b0">Library Access</a>.

<b>Windows Media Player 10 Mobile: </b>This method always returns E_INVALIDARG.




## -see-also




<a href="https://msdn.microsoft.com/323a6841-ffbd-4bbb-ac04-1d121cf5bd06">IWMPCdrom Interface</a>



<a href="https://msdn.microsoft.com/1b17c405-0887-4948-b375-c1ebcf2a72b3">IWMPCdrom::eject</a>



<a href="https://msdn.microsoft.com/ba55ac32-149d-4f7b-a2bb-1fdb0be806cd">IWMPCdromCollection Interface</a>



<a href="https://msdn.microsoft.com/07ca80a3-5175-4b1f-b83c-0df41a010cbf">IWMPSettings2::get_mediaAccessRights</a>



<a href="https://msdn.microsoft.com/925a4c0b-d613-4248-a341-bfc51d02cb85">IWMPSettings2::requestMediaAccessRights</a>
 

 

