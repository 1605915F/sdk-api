---
UID: NN:certexit.ICertExit
title: ICertExit
author: windows-sdk-content
description: Provides communications between the Certificate Services server and an exit module.
old-location: security\icertexit.htm
tech.root: seccrypto
ms.assetid: 731c4f3c-20b4-4f3d-8241-a94cdf656fe5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICertExit, ICertExit interface [Security], ICertExit interface [Security],described, _certsrv_icertexit, certexit/ICertExit, security.icertexit
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: certexit.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certexit.h
api_name:
 - ICertExit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertExit interface


## -description


The <b>ICertExit</b> interface  provides communications between  the Certificate Services server and an exit module.
<div class="alert"><b>Note</b>  The exit module can communicate with the Certificate Services server by using the <a href="https://msdn.microsoft.com/en-us/library/Aa385055(v=VS.85).aspx">ICertServerExit</a> interface.</div><div> </div>The Certificate Services server calls the <b>ICertExit</b> methods to perform the following tasks:<ul>
<li>Initialize the Certificate Services server.</li>
<li>Notify the exit module of an event such as certificate issuance, <a href="https://msdn.microsoft.com/en-us/library/ms721572(v=VS.85).aspx">certificate revocation list</a> (CRL) issuance, or server shutdown, has occurred.</li>
<li>Retrieve a description of the exit module.</li>
</ul>


<b>ICertExit</b> is defined in Certexit.h. When you create your program, however, use Certsrv.h as the include file.

Certificate Services interfaces support both apartment-threading and free-threading models. For better throughput, free threading is recommended.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICertExit</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>ICertExit</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>ICertExit</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa385023(v=VS.85).aspx">GetDescription</a>
</td>
<td align="left" width="63%">
Returns a description of the exit module and its function.</p> (Inherited from <b>ICertExit</b><a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">ICertExit2</a>
<a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">CCertExit2</a>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa385025(v=VS.85).aspx">Initialize</a>
</td>
<td align="left" width="63%">
Called by the server engine when it initializes itself.</p> (Inherited from <b>ICertExit</b><a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">ICertExit2</a>
<a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">CCertExit2</a>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa385026(v=VS.85).aspx">Notify</a>
</td>
<td align="left" width="63%">
Called by the server engine to notify an exit module that an event has occurred.</p> (Inherited from <b>ICertExit</b><a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">ICertExit2</a>
<a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">CCertExit2</a>)</td>
</tr>
</table> 


## -remarks



Implementers of <b>ICertExit</b> should also implement 
<a href="https://msdn.microsoft.com/en-us/library/Aa385029(v=VS.85).aspx">ICertManageModule</a>. Additionally, the ProgID for a class implementing <b>ICertExit</b> must conform to a naming convention. Specifically, the ProgID must be of the form:

<b>"</b><i>MyApp</i><b>.Exit"</b>

Where <i>MyApp</i> is a specifier that identifies the application. For example, in C++, the following code could be used in the DECLARE_REGISTRY macro of a class (CMyCertExitModule) which implements <b>ICertExit</b>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>DECLARE_REGISTRY(
    CMyCertExitModule,
    L"MyCode.Exit.1",
    L"MyCode.Exit",
    IDS_CERTEXITMODULE_DESC,
    THREADFLAGS_BOTH)</pre>
</td>
</tr>
</table></span></div>
For the previous sample, the IDS_CERTEXITMODULE_DESC value is an application-specific identifier in the resource file (.rc) for a string that describes the class.

String constants defined in Certmod.h can be used to simplify following the naming convention.

<table>
<tr>
<th>Constant</th>
<th>Value</th>
</tr>
<tr>
<td>
<b>wszCERTEXITMODULE_POSTFIX</b>

</td>
<td>
TEXT(".Exit")

</td>
</tr>
</table>
 

No more than one Visual Basic Scripting Edition exit module may be registered on the Certificate Services server at one time. If more than one Visual Basic Scripting Edition exit module is registered, the Certification Authority MMC snap-in, Certificate Services application, or certutil command line program may produce errors. Note that the Visual Basic Scripting Edition development environment automatically registers a DLL when it is successfully built. As a result, you may encounter this situation when one Visual Basic Scripting Edition exit module is already registered and another Visual Basic Scripting Edition exit module is created. To avoid this situation, you must unregister one of the Visual Basic Scripting Edition exit modules, by means of the command-line instruction <b>regsvr32 /u </b><i>FileName</i><b>.dll</b>, where <i>FileName</i>.dll is the name of the Visual Basic Scripting Edition exit module that is not intended to be made active.

Implementers of <b>ICertExit</b> in Visual Basic Scripting Edition must name their project in the form:

<b>"</b><i>MyApp</i><b>"</b>

Where <i>MyApp</i> is a specifier that identifies the application; further, the class implementing <b>ICertExit</b> must be named <b>"Exit"</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa385055(v=VS.85).aspx">ICertServerExit</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

