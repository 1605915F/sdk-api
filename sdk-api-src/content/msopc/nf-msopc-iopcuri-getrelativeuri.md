---
UID: NF:msopc.IOpcUri.GetRelativeUri
title: IOpcUri::GetRelativeUri (msopc.h)
author: windows-sdk-content
description: Forms a relative URI for a specified part, relative to the URI represented by the current OPC URI object.
old-location: opc\iopcuri_getrelativeuri.htm
tech.root: OPC
ms.assetid: ce98b0a6-f4b3-4f49-897a-f144af7dfc49
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRelativeUri, GetRelativeUri method [Open Packaging Conventions], GetRelativeUri method [Open Packaging Conventions],IOpcUri interface, IOpcUri interface [Open Packaging Conventions],GetRelativeUri method, IOpcUri.GetRelativeUri, IOpcUri::GetRelativeUri, msopc/IOpcUri::GetRelativeUri, opc.iopcuri_getrelativeuri
ms.topic: method
req.header: msopc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Opcparturi.idl
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
 - msopc.h
api_name:
 - IOpcUri.GetRelativeUri
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOpcUri::GetRelativeUri


## -description


 Forms a relative URI for a specified part, relative to the URI represented by the current OPC URI object.


## -parameters




### -param targetPartUri [in]

A pointer to the <a href="https://msdn.microsoft.com/81123212-7a32-4833-b81f-8454a544327d">IOpcPartUri</a> interface of the part URI object that represents the part name from which the relative URI is formed.


### -param relativeUri [out, retval]

A pointer to the <a href="http://go.microsoft.com/fwlink/p/?linkid=116163">IUri</a> interface of the URI of the part, relative to the current OPC URI object.


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
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
 At least one of the <i>targetPartUri</i>, and <i>relativePartUri</i> parameters is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>CreateUri</b> function error</b></dt>
</dl>
</td>
<td width="60%">
An <b>HRESULT</b> error code from the <a href="https://msdn.microsoft.com/library/ms775098(v=VS.85).aspx">CreateUri</a> function. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WinINet error</b></dt>
</dl>
</td>
<td width="60%">
An <b>HRESULT</b> error code from a  <a href="https://msdn.microsoft.com/dd2f8246-ea82-49cb-973f-157fb77c8c08">WinINet</a> API. 

</td>
</tr>
</table>
 




## -remarks



Example input and output:


<table>
<tr>
<th>Input <a href="https://msdn.microsoft.com/81123212-7a32-4833-b81f-8454a544327d">IOpcPartUri</a> represents</th>
<th>Current <a href="https://msdn.microsoft.com/35ce7946-f7e7-4ac3-852f-e3fcca23d6d4">IOpcUri</a> represents</th>
<th>Returned relative <a href="http://go.microsoft.com/fwlink/p/?linkid=116163">IUri</a> represents</th>
</tr>
<tr>
<td>/mydoc/markup/page.xml</td>
<td>	/mydoc/markup/picture.jpg	</td>
<td>picture.jpg</td>
</tr>
<tr>
<td>/mydoc/markup/page.xml</td>
<td>/mydoc/picture.jpg</td>
<td>../picture.jpg</td>
</tr>
<tr>
<td>/mydoc/markup/page.xml</td>
<td>/mydoc/images/pictures.jpg</td>
<td>../images/pictures.jpg</td>
</tr>
</table>
 



<h3><a id="Support_on__Previous_Windows_Versions"></a><a id="support_on__previous_windows_versions"></a><a id="SUPPORT_ON__PREVIOUS_WINDOWS_VERSIONS"></a>Support on  Previous Windows Versions</h3>
The behavior and performance of this method is the same on all supported Windows versions. For more information, see <a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>, and <a href="https://msdn.microsoft.com/661f88f9-e5ba-412d-8cb4-f3f186568b74">Platform Update for Windows Vista</a>.


#### Thread Safety

Packaging objects are not thread-safe.

For more information, see the <a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>.




## -see-also




<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/35ce7946-f7e7-4ac3-852f-e3fcca23d6d4">IOpcUri</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/b4cd8f69-3559-46a0-95ec-6fcaab21959c">Packaging Errors</a>



<a href="https://msdn.microsoft.com/661f88f9-e5ba-412d-8cb4-f3f186568b74">Platform Update for Windows Vista</a>



<b>Reference</b>
 

 

