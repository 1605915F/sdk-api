---
UID: NF:msopc.IOpcFactory.CreatePackage
title: IOpcFactory::CreatePackage (msopc.h)
author: windows-sdk-content
description: Creates a package object that represents an empty package.
old-location: opc\iopcfactory_createpackage.htm
tech.root: OPC
ms.assetid: 9cd4ef3a-f890-40d5-a398-cb8f9746c380
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreatePackage, CreatePackage method [Open Packaging Conventions], CreatePackage method [Open Packaging Conventions],IOpcFactory interface, IOpcFactory interface [Open Packaging Conventions],CreatePackage method, IOpcFactory.CreatePackage, IOpcFactory::CreatePackage, msopc/IOpcFactory::CreatePackage, opc.iopcfactory_createpackage
ms.topic: method
req.header: msopc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Msopc.idl
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
 - IOpcFactory.CreatePackage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOpcFactory::CreatePackage


## -description


Creates a package object that represents an empty package.


## -parameters




### -param package [out, retval]

A pointer to the <a href="https://msdn.microsoft.com/e7052dd2-c910-41d8-a58a-8f3e68e09dd0">IOpcPackage</a> interface of the package object that represents an empty package.


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
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
This method is not implemented for this version of Windows.

</td>
</tr>
</table>
 




## -remarks



<h3><a id="Support_on_Previous_Versions_of_Windows"></a><a id="support_on_previous_versions_of_windows"></a><a id="SUPPORT_ON_PREVIOUS_VERSIONS_OF_WINDOWS"></a>Support on Previous Versions of Windows</h3>
This method is not supported on versions of Windows prior to Windows 7. For more information, see <a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>, and <a href="https://msdn.microsoft.com/661f88f9-e5ba-412d-8cb4-f3f186568b74">Platform Update for Windows Vista</a>.


#### Thread Safety

Packaging objects are not thread-safe.

For more information, see the <a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>.




## -see-also




<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/0a265a0a-c109-4afc-a0ad-d3ee31757aa1">IOpcFactory</a>



<a href="https://msdn.microsoft.com/8063fcb5-4629-4b6b-857b-bb22f0572f0d">Music Bundle Sample</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/f42a8581-dcaa-43a6-997f-984303a32ff3">Packages Overview</a>



<a href="https://msdn.microsoft.com/cb35d87e-bbec-42d3-9f9d-d1cf36f39419">Packaging API Programming Guide</a>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/b4cd8f69-3559-46a0-95ec-6fcaab21959c">Packaging Errors</a>



<a href="https://msdn.microsoft.com/661f88f9-e5ba-412d-8cb4-f3f186568b74">Platform Update for Windows Vista</a>



<b>Reference</b>
 

 

