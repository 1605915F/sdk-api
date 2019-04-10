---
UID: NN:certenroll.IX509CertificateTemplateWritable
title: IX509CertificateTemplateWritable (certenroll.h)
author: windows-sdk-content
description: The IX509CertificateTemplateWritable interface enables you to add a template to or delete it from a template store. Currently, Active Directory is the only available store.
old-location: security\ix509certificatetemplatewritable.htm
tech.root: seccertenroll
ms.assetid: 87660b16-06a8-4a71-8669-24521f1399e4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IX509CertificateTemplateWritable, IX509CertificateTemplateWritable interface [Security], IX509CertificateTemplateWritable interface [Security],described, certenroll/IX509CertificateTemplateWritable, security.ix509certificatetemplatewritable
ms.topic: interface
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: CertEnroll.dll
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - IX509CertificateTemplateWritable
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509CertificateTemplateWritable interface


## -description


The <b>IX509CertificateTemplateWritable</b> interface enables you to add a template to or delete it from a template store. Currently, Active Directory is the only available store.



## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IX509CertificateTemplateWritable</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IX509CertificateTemplateWritable</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>IX509CertificateTemplateWritable</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ee7d5640-8d06-4a1a-bce2-f76ee6276207">Commit</a>
</td>
<td align="left" width="63%">
Deletes a template from or saves it to Active Directory.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d70cfb65-403f-4a58-8882-393029111552">Initialize</a>
</td>
<td align="left" width="63%">
Initializes an <b>IX509CertificateTemplateWritable</b> object from a template.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IX509CertificateTemplateWritable</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/df665957-c276-4e46-8838-76010146e4d7">Property</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
Specifies or retrieves a property value for the <b>IX509CertificateTemplateWritable</b> object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/35eef4e5-fcd9-4017-9d15-d8d418e063e7">Template</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Retrieves a copy of the template used to initialize the <b>IX509CertificateTemplateWritable</b> object.

</td>
</tr>
</table> 

