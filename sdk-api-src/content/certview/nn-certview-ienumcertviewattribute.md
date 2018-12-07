---
UID: NN:certview.IEnumCERTVIEWATTRIBUTE
title: IEnumCERTVIEWATTRIBUTE
author: windows-sdk-content
description: Represents an attribute-enumeration sequence that contains the certificate attributes for the current row of the row-enumeration sequence.
old-location: security\ienumcertviewattribute.htm
tech.root: seccrypto
ms.assetid: fc1eb29d-27d9-4331-b588-dc0632b3db6a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumCERTVIEWATTRIBUTE, IEnumCERTVIEWATTRIBUTE interface [Security], IEnumCERTVIEWATTRIBUTE interface [Security],described, _certsrv_ienumcertviewattribute, certview/IEnumCERTVIEWATTRIBUTE, security.ienumcertviewattribute
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: certview.h
req.include-header: Certsrv.h
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.lib: Certidl.lib
req.dll: Certadm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certadm.dll
api_name:
 - IEnumCERTVIEWATTRIBUTE
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumCERTVIEWATTRIBUTE interface


## -description


The <b>IEnumCERTVIEWATTRIBUTE</b> interface represents an attribute-enumeration sequence that contains the   certificate attributes for the current row of the row-enumeration sequence.

The attribute-enumeration sequence is obtained by a call to 
the <a href="https://msdn.microsoft.com/en-us/library/Aa386234(v=VS.85).aspx">IEnumCERTVIEWROW::EnumCertViewAttribute</a> method. After this enumeration sequence is obtained, the methods of the <b>IEnumCERTVIEWATTRIBUTE</b> interface can be used to perform the following tasks:<ul>
<li>Navigate through the enumeration of certificate attributes.</li>
<li>Retrieve the name and value of the attributes in the enumeration.</li>
<li>Clone an exact copy of the certificate attribute object.</li>
</ul>


<b>IEnumCERTVIEWATTRIBUTE</b> is defined in Certview.h. When you create your program, however, use Certsrv.h as the include file. Certadm.dll provides the <b>IEnumCERTVIEWATTRIBUTE</b> interface. The type information for this interface is also in Certadml.dll, which is shipped with the Platform Software Development Kit (SDK).

Certificate Services interfaces support both apartment-threading and free-threading models. For better throughput, free threading is recommended.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumCERTVIEWATTRIBUTE</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IEnumCERTVIEWATTRIBUTE</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>IEnumCERTVIEWATTRIBUTE</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386160(v=VS.85).aspx">Clone</a>
</td>
<td align="left" width="63%">
Creates a copy of the attribute-enumeration sequence object in its current state.</p> (Inherited from <b>IEnumCERTVIEWATTRIBUTE</b><b>IEnumCETVIEWATTRIBUTE</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386164(v=VS.85).aspx">GetName</a>
</td>
<td align="left" width="63%">
Retrieves the name of the current attribute in the attribute-enumeration sequence.</p> (Inherited from <b>IEnumCERTVIEWATTRIBUTE</b><b>IEnumCETVIEWATTRIBUTE</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386166(v=VS.85).aspx">GetValue</a>
</td>
<td align="left" width="63%">
Retrieves the value of the current attribute in the attribute-enumeration sequence.</p> (Inherited from <b>IEnumCERTVIEWATTRIBUTE</b><b>IEnumCETVIEWATTRIBUTE</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386168(v=VS.85).aspx">Next</a>
</td>
<td align="left" width="63%">
Moves to the next  attribute in the attribute-enumeration sequence.</p> (Inherited from <b>IEnumCERTVIEWATTRIBUTE</b><b>IEnumCETVIEWATTRIBUTE</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386170(v=VS.85).aspx">Reset</a>
</td>
<td align="left" width="63%">
Moves to the beginning of the attribute-enumeration sequence.</p> (Inherited from <b>IEnumCERTVIEWATTRIBUTE</b><b>IEnumCETVIEWATTRIBUTE</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa386172(v=VS.85).aspx">Skip</a>
</td>
<td align="left" width="63%">
Skips a specified number of attributes in the attribute-enumeration sequence.</p> (Inherited from <b>IEnumCERTVIEWATTRIBUTE</b><b>IEnumCETVIEWATTRIBUTE</b>)</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386234(v=VS.85).aspx">IEnumCERTVIEWROW::EnumCertViewAttribute</a>
 

 

