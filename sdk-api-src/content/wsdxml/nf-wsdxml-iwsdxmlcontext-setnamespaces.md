---
UID: NF:wsdxml.IWSDXMLContext.SetNamespaces
title: IWSDXMLContext::SetNamespaces
author: windows-sdk-content
description: Associates custom namespaces with the XML context object.
old-location: ncd\iwsdxmlcontext_setnamespaces_method.htm
tech.root: wsdapi
ms.assetid: 94ec94d1-e0d8-42cb-993f-6da9c8df1a47
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWSDXMLContext interface,SetNamespaces method, IWSDXMLContext.SetNamespaces, IWSDXMLContext::SetNamespaces, SetNamespaces, SetNamespaces method, SetNamespaces method,IWSDXMLContext interface, ncd.iwsdxmlcontext_setnamespaces_method, wsdxml/IWSDXMLContext::SetNamespaces
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wsdxml.h
req.include-header: Wsdapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WsdXml.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Wsdapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wsdapi.dll
api_name:
 - IWSDXMLContext.SetNamespaces
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWSDXMLContext::SetNamespaces


## -description


Associates custom namespaces with the XML context object. 

This method should only be called by <a href="https://msdn.microsoft.com/76dffca8-bb84-4384-a9e8-120a4cf2acac">generated code</a>, and should not be called directly by a WSDAPI client. Instead, the code generator will provide wrappers that access this method properly.


## -parameters




### -param pNamespaces [in]

An array of <a href="https://msdn.microsoft.com/dcf27f38-e628-4b0c-859c-ad12d3ed0924">WSDXML_NAMESPACE</a> structures.


### -param wNamespacesCount [in]

The number of namespaces in the <i>pNamespaces</i> array.


### -param bLayerNumber [in]

The layer number associated with the <a href="https://msdn.microsoft.com/76dffca8-bb84-4384-a9e8-120a4cf2acac">generated service code</a>.


## -returns



Possible return values include, but are not limited to, the following:

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
Method completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i>pNamespaces</i> is <b>NULL</b> or  <i>bLayerNumber</i> is greater than or equal to WSD_XMLCONTEXT_NUM_LAYERS (16).

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory to complete the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The method failed.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/131fa170-4c19-4a7b-82e0-e9677b7f767a">IWSDXMLContext</a>
 

 

