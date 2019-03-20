---
UID: NF:devicetopology.IAudioOutputSelector.SetSelection
title: IAudioOutputSelector::SetSelection (devicetopology.h)
author: windows-sdk-content
description: The SetSelection method selects one of the outputs of the output selector.
old-location: coreaudio\iaudiooutputselector_setselection.htm
tech.root: CoreAudio
ms.assetid: e81d54f4-1451-4bd0-be06-28ff01fb65ab
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAudioOutputSelector interface [Core Audio],SetSelection method, IAudioOutputSelector.SetSelection, IAudioOutputSelector::SetSelection, IAudioOutputSelectorSetSelection, SetSelection, SetSelection method [Core Audio], SetSelection method [Core Audio],IAudioOutputSelector interface, coreaudio.iaudiooutputselector_setselection, devicetopology/IAudioOutputSelector::SetSelection
ms.topic: method
req.header: devicetopology.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Devicetopology.h
api_name:
 - IAudioOutputSelector.SetSelection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAudioOutputSelector::SetSelection


## -description



The <b>SetSelection</b> method selects one of the outputs of the output selector.




## -parameters




### -param nIdSelect [in]

The new selector output. The caller should set this parameter to the local ID of a part that has a direct link to one of the selector outputs.


### -param pguidEventContext [in]

Context value for the <a href="https://msdn.microsoft.com/a2f32cb9-3c8b-4b44-96a2-dd70afcca71a">IControlChangeNotify::OnNotify</a> method. This parameter points to an event-context GUID. If the <b>SetSelection</b> call changes the state of the output-selector control, all clients that have registered <a href="https://msdn.microsoft.com/e50e13c2-1ef3-46f6-8c53-f99cc1631a79">IControlChangeNotify</a> interfaces with that control receive notifications. In its implementation of the <b>OnNotify</b> method, a client can inspect the event-context GUID to discover whether it or another client is the source of the control-change event. If the caller supplies a <b>NULL</b> pointer for this parameter, the client's notification method receives a <b>NULL</b> context pointer.


## -returns



If the method succeeds, it returns S_OK. If it fails, possible return codes include, but are not limited to, the values shown in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Parameter <i>nIdSelect</i> is not the local ID of a part at a selector output.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Out of memory.

</td>
</tr>
</table>
 




## -remarks



A local ID is a number that uniquely identifies a part among all parts in a device topology. To obtain the local ID of a part, call the <a href="https://msdn.microsoft.com/d5ca4908-1822-485c-a04a-0eeee1e384a8">IPart::GetLocalId</a> method on the part object.




## -see-also




<a href="https://msdn.microsoft.com/571a44b6-972f-4d75-a31f-0e02cf728764">IAudioOutputSelector Interface</a>



<a href="https://msdn.microsoft.com/d5ca4908-1822-485c-a04a-0eeee1e384a8">IPart::GetLocalId</a>
 

 

