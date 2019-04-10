---
UID: NS:qosobjs._QOS_DS_CLASS
title: QOS_DS_CLASS (qosobjs.h)
author: windows-sdk-content
description: The traffic control object QOS_DS_CLASS enables application developers to override the default Diffserv code point (DSCP) value for the IP packets associated with a given flow. By default, the DSCP value is derived from the flow's ServiceType.
old-location: qos\qos_ds_class.htm
tech.root: QOS
ms.assetid: 56eca8ef-2b6e-4380-869c-bf1a4c8fdb1f
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPQOS_DS_CLASS, LPQOS_DS_CLASS, LPQOS_DS_CLASS structure pointer [QOS], QOS_DS_CLASS, QOS_DS_CLASS structure [QOS], _gqos_qos_ds_class, qos.qos_ds_class, qosobjs/LPQOS_DS_CLASS, qosobjs/QOS_DS_CLASS"
ms.topic: struct
req.header: qosobjs.h
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
 - HeaderDef
api_location:
 - QosObjs.h
api_name:
 - QOS_DS_CLASS
product: Windows
targetos: Windows
req.typenames: QOS_DS_CLASS, *LPQOS_DS_CLASS
req.redist: 
---

# QOS_DS_CLASS structure


## -description


The traffic control object 
<b>QOS_DS_CLASS</b> enables application developers to override the default Diffserv code point (DSCP) value for the IP packets associated with a given flow. By default, the DSCP value is derived from the flow's ServiceType.


## -struct-fields




### -field ObjectHdr

The QOS object 
<a href="https://msdn.microsoft.com/a2021d70-e7ef-4c2a-8800-1a1d7540ce02">QOS_OBJECT_HDR</a>. The object type for this traffic control object should be 
<b>QOS_OBJECT_DS_CLASS</b>.


### -field DSField

User priority value for the flow. The valid range is 0x00 through 0x3F. The following settings are chosen (by default) when the 
<b>QOS_DS_CLASS</b> traffic control object is not used. 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0</dt>
</dl>
</td>
<td width="60%">
ServiceTypeBestEffort, ServiceTypeQualitative

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0x18</dt>
</dl>
</td>
<td width="60%">
ServiceTypeControlledLoad

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0x28</dt>
</dl>
</td>
<td width="60%">
ServiceTypeGuaranteed

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0x30</dt>
</dl>
</td>
<td width="60%">
ServiceTypeNetworkControl

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0x00</dt>
</dl>
</td>
<td width="60%">
Non-conformant traffic

</td>
</tr>
</table>
 


## -see-also




<a href="https://msdn.microsoft.com/3d1035dc-0e46-46f4-abb3-26100356b60d">QOS_DIFFSERV</a>



<a href="https://msdn.microsoft.com/732cfbec-4175-4397-854f-0d2a930e11bc">QOS_DIFFSERV_RULE</a>



<a href="https://msdn.microsoft.com/a2021d70-e7ef-4c2a-8800-1a1d7540ce02">QOS_OBJECT_HDR</a>



<a href="https://msdn.microsoft.com/60c6492f-ddcf-401c-8121-2349b89eb223">QOS_TRAFFIC_CLASS</a>
 

 

