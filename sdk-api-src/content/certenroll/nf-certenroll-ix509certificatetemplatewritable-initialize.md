---
UID: NF:certenroll.IX509CertificateTemplateWritable.Initialize
title: IX509CertificateTemplateWritable::Initialize (certenroll.h)
author: windows-sdk-content
description: Initializes an IX509CertificateTemplateWritable object from a template.
old-location: security\ix509certificatetemplatewritable_initialize.htm
tech.root: seccertenroll
ms.assetid: d70cfb65-403f-4a58-8882-393029111552
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IX509CertificateTemplateWritable interface [Security],Initialize method, IX509CertificateTemplateWritable.Initialize, IX509CertificateTemplateWritable::Initialize, Initialize, Initialize method [Security], Initialize method [Security],IX509CertificateTemplateWritable interface, certenroll/IX509CertificateTemplateWritable::Initialize, security.ix509certificatetemplatewritable_initialize
ms.topic: method
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certenroll.idl
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
 - Certenroll.h
api_name:
 - IX509CertificateTemplateWritable.Initialize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IX509CertificateTemplateWritable::Initialize


## -description


The <b>Initialize</b> method initializes an <a href="https://msdn.microsoft.com/87660b16-06a8-4a71-8669-24521f1399e4">IX509CertificateTemplateWritable</a> object from a template.


## -parameters




### -param pValue [in]

Pointer to an <a href="https://msdn.microsoft.com/56122d92-7e38-4eaa-b2f5-713adc81e68e">IX509CertificateTemplate</a> interface that represents a certificate request template.


## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table.  For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_POINTER</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The <i>pValue</i> parameter cannot be <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOINTERFACE </b></dt>
</dl>
</td>
<td width="60%">
The <i>pValue</i> parameter does not point to an <a href="https://msdn.microsoft.com/56122d92-7e38-4eaa-b2f5-713adc81e68e">IX509CertificateTemplate</a> interface.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>HRESULT_FROM_WIN32(ERROR_ALREADY_INITIALIZED)</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/87660b16-06a8-4a71-8669-24521f1399e4">IX509CertificateTemplateWritable</a> has already been initialized.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/87660b16-06a8-4a71-8669-24521f1399e4">IX509CertificateTemplateWritable</a>
 

 

