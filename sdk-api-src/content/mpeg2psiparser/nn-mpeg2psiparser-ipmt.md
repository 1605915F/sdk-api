---
UID: NN:mpeg2psiparser.IPMT
title: IPMT
author: windows-sdk-content
description: The IPMT interface enables the client to get information from a program map table (PMT).
old-location: mstv\ipmt.htm
tech.root: mstv
ms.assetid: 0dbd4cc3-5ef3-4c71-ba3f-149d5050ba24
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPMT, IPMT interface [Microsoft TV Technologies], IPMT interface [Microsoft TV Technologies],described, IPMTInterface, mpeg2psiparser/IPMT, mstv.ipmt
ms.topic: interface
req.header: mpeg2psiparser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mpeg2PsiParser.h
api_name:
 - IPMT
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPMT interface


## -description



The <b>IPMT</b> interface enables the client to get information from a program map table (PMT). The <a href="https://msdn.microsoft.com/cd9a3fb0-4bdc-499b-9db9-85dce50dd24b">IAtscPsipParser::GetPMT</a> method returns a pointer to this interface.

The PMT may contain one or more table-wide descriptors. In addition, each record in the PMT may have one or more descriptors. To get the table-wide descriptors, use the <b>GetTableDescriptorByIndex</b> or <b>GetTableDescriptorByTag</b> method. To get the record descriptors, use the <b>GetRecordDescriptorByIndex</b> or <b>GetRecordDescriptorByTag</b> method.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IPMT</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IPMT</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IPMT</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694821(v=VS.85).aspx">ConvertNextToCurrent</a>
</td>
<td align="left" width="63%">
Converts a <i>next</i> table to a <i>current</i> table.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694822(v=VS.85).aspx">GetCountOfRecords</a>
</td>
<td align="left" width="63%">
Returns the number of records in the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694823(v=VS.85).aspx">GetCountOfTableDescriptors</a>
</td>
<td align="left" width="63%">
Returns the number of table-wide descriptors in the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694824(v=VS.85).aspx">GetNextTable</a>
</td>
<td align="left" width="63%">
Retrieves the <i>next</i> table that follows the current table.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694825(v=VS.85).aspx">GetPcrPid</a>
</td>
<td align="left" width="63%">
Returns the packet identifier (PID) of the packets that contain the Program Clock Reference (PCR) fields for this program.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694826(v=VS.85).aspx">GetProgramNumber</a>
</td>
<td align="left" width="63%">
Returns the program number for the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694827(v=VS.85).aspx">GetRecordCountOfDescriptors</a>
</td>
<td align="left" width="63%">
Returns the number of descriptors for a record in the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1e37db4b-1b86-4b34-8f93-642bb603789e">GetRecordDescriptorByIndex</a>
</td>
<td align="left" width="63%">
Retrieves a descriptor for a specified record in the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694829(v=VS.85).aspx">GetRecordDescriptorByTag</a>
</td>
<td align="left" width="63%">
Searches a record in the PMT for a descriptor with a specified descriptor tag.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694830(v=VS.85).aspx">GetRecordElementaryPid</a>
</td>
<td align="left" width="63%">
Returns the PID for a given elementary stream in the program.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694831(v=VS.85).aspx">GetRecordStreamType</a>
</td>
<td align="left" width="63%">
Returns the stream type for a given elementary stream in the program.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/31442c1f-0921-49b8-ab38-d75ccc2c4f0e">GetTableDescriptorByIndex</a>
</td>
<td align="left" width="63%">
Retrieves a table-wide descriptor for the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694833(v=VS.85).aspx">GetTableDescriptorByTag</a>
</td>
<td align="left" width="63%">
Searches the PMT for a table-wide descriptor with the specified descriptor tag.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694834(v=VS.85).aspx">GetVersionNumber</a>
</td>
<td align="left" width="63%">
Returns the version number for the PMT.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694835(v=VS.85).aspx">Initialize</a>
</td>
<td align="left" width="63%">
Initializes the object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694836(v=VS.85).aspx">QueryMPEInfo</a>
</td>
<td align="left" width="63%">
Returns the Multi-Protocol Encapsulation (MPE) information in the PMT, if any.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694837(v=VS.85).aspx">QueryServiceGatewayInfo</a>
</td>
<td align="left" width="63%">
Returns the DSM-CC service gateway information in the PMT, if any.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694838(v=VS.85).aspx">RegisterForNextTable</a>
</td>
<td align="left" width="63%">
Registers the client to be notified when a <i>next</i> table arrives that will replace the current table.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694839(v=VS.85).aspx">RegisterForWhenCurrent</a>
</td>
<td align="left" width="63%">
Registers the client to be notified when the table becomes current.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/07d18f73-e852-4c88-a2e2-e8f4198ca799">BDA Interfaces</a>
 

 

