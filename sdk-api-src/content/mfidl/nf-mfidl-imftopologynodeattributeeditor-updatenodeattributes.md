---
UID: NF:mfidl.IMFTopologyNodeAttributeEditor.UpdateNodeAttributes
title: IMFTopologyNodeAttributeEditor::UpdateNodeAttributes (mfidl.h)
author: windows-sdk-content
description: Updates the attributes of one or more nodes in the current topology.
old-location: mf\imftopologynodeattributeeditor_updatenodeattributes.htm
tech.root: medfound
ms.assetid: a769b0bd-a43f-478b-a6e4-bbef05942616
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IMFTopologyNodeAttributeEditor interface [Media Foundation],UpdateNodeAttributes method, IMFTopologyNodeAttributeEditor.UpdateNodeAttributes, IMFTopologyNodeAttributeEditor::UpdateNodeAttributes, UpdateNodeAttributes, UpdateNodeAttributes method [Media Foundation], UpdateNodeAttributes method [Media Foundation],IMFTopologyNodeAttributeEditor interface, a769b0bd-a43f-478b-a6e4-bbef05942616, mf.imftopologynodeattributeeditor_updatenodeattributes, mfidl/IMFTopologyNodeAttributeEditor::UpdateNodeAttributes
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfuuid.lib
 - mfuuid.dll
api_name:
 - IMFTopologyNodeAttributeEditor.UpdateNodeAttributes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFTopologyNodeAttributeEditor::UpdateNodeAttributes


## -description



Updates the attributes of one or more nodes in the current topology.




## -parameters




### -param TopoId [in]

Reserved.


### -param cUpdates [in]

The number of elements in the <i>pUpdates</i> array.


### -param pUpdates [in]

Pointer to an array of <a href="https://msdn.microsoft.com/94c89067-9b3e-4d24-9192-a68e284c5d99">MFTOPONODE_ATTRIBUTE_UPDATE</a> structures. Each element of the array updates one attribute on a node.


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



Currently the only attribute that can be updated is the <a href="https://msdn.microsoft.com/c1022538-ea9f-41e9-9075-c106e8b16b7b">MF_TOPONODE_MEDIASTOP</a> attribute. The method ignores any other attributes.




## -see-also




<a href="https://msdn.microsoft.com/9ab384b9-0ce9-428c-a683-b09dbd4e07d9">IMFTopologyNodeAttributeEditor</a>
 

 

