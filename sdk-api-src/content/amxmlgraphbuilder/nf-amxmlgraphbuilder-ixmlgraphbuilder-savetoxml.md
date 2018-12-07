---
UID: NF:amxmlgraphbuilder.IXMLGraphBuilder.SaveToXML
title: IXMLGraphBuilder::SaveToXML
author: windows-sdk-content
description: The SaveToXML method saves a filter graph to an XML element.
old-location: dshow\ixmlgraphbuilder_savetoxml.htm
tech.root: DirectShow
ms.assetid: 02f710a4-3d13-46b0-b00d-4ffd2b4c3157
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXMLGraphBuilder interface [DirectShow],SaveToXML method, IXMLGraphBuilder.SaveToXML, IXMLGraphBuilder::SaveToXML, IXMLGraphBuilderSaveToXML, SaveToXML, SaveToXML method [DirectShow], SaveToXML method [DirectShow],IXMLGraphBuilder interface, amxmlgraphbuilder/IXMLGraphBuilder::SaveToXML, dshow.ixmlgraphbuilder_savetoxml
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: amxmlgraphbuilder.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - amxmlgraphbuilder.h
api_name:
 - IXMLGraphBuilder.SaveToXML
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXMLGraphBuilder::SaveToXML


## -description



The <b>SaveToXML</b> method saves a filter graph to an XML element.


<div class="alert"><b>Note</b>  Support for this interface was removed in Windows 7. New applications should not use this interface.</div><div> </div>

## -parameters




### -param pGraph [in]

Pointer to the Filter Graph Manager's <a href="https://msdn.microsoft.com/54ed8ac8-4821-4c0c-9fb9-789c70dbca37">IGraphBuilder</a> interface.


### -param pbstrxml [out]

Pointer to a <b>BSTR</b> that receives the XML element. The caller must release the string by calling <b>SysFreeString</b>.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/c30a8b33-7783-4987-aa65-ccba476ea937">IXMLGraphBuilder Interface</a>
 

 

