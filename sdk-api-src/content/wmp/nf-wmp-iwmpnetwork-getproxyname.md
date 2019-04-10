---
UID: NF:wmp.IWMPNetwork.getProxyName
title: IWMPNetwork::getProxyName (wmp.h)
author: windows-sdk-content
description: The getProxyName method retrieves the name of the proxy server being used.
old-location: wmp\iwmpnetwork_getproxyname.htm
tech.root: WMP
ms.assetid: 7bf3adaa-a89d-4ffe-8233-a9c606b39350
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMPNetwork interface [Windows Media Player],getProxyName method, IWMPNetwork.getProxyName, IWMPNetwork::getProxyName, IWMPNetworkgetProxyName, getProxyName, getProxyName method [Windows Media Player], getProxyName method [Windows Media Player],IWMPNetwork interface, wmp.iwmpnetwork_getproxyname, wmp/IWMPNetwork::getProxyName
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
 - IWMPNetwork.getProxyName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPNetwork::getProxyName


## -description



The <b>getProxyName</b> method retrieves the name of the proxy server being used.




## -parameters




### -param bstrProtocol [in]

<b>BSTR</b> containing the protocol name. For a list of supported protocols, see <a href="https://msdn.microsoft.com/2672372c-0b42-437e-8b96-83b6e5200fd3">Supported Protocols and File Types</a>.


### -param pbstrProxyName [out]

Pointer to a <b>BSTR</b> containing the name of the proxy server being used. The value retrieved is meaningful only when <b>IWMPNetwork::getProxySettings</b> retrieves a value of 2 (use manual settings).


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



This method fails unless the calling application is running on the local computer or intranet.

<b>Windows Media Player 10 Mobile:</b> This method always returns E_INVALIDARG.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd563461(v=VS.85).aspx">IWMPNetwork Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563467(v=VS.85).aspx">IWMPNetwork::getProxySettings</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563488(v=VS.85).aspx">IWMPNetwork::setProxyName</a>
 

 

