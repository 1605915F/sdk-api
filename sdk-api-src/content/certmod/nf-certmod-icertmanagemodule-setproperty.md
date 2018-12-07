---
UID: NF:certmod.ICertManageModule.SetProperty
title: ICertManageModule::SetProperty
author: windows-sdk-content
description: Allows a module to set a property value.
old-location: security\icertmanagemodule_setproperty.htm
tech.root: seccrypto
ms.assetid: 582ace4a-da88-41b7-86dd-d6a74fc9e97a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CCertManageModule object [Security],SetProperty method, Copyright, Description, File Version, ICertManageModule interface [Security],SetProperty method, ICertManageModule.SetProperty, ICertManageModule::SetProperty, Name, Product Version, SetProperty, SetProperty method [Security], SetProperty method [Security],CCertManageModule object, SetProperty method [Security],ICertManageModule interface, _certsrv_icertmanagemodule_setproperty, certmod/ICertManageModule::SetProperty, security.icertmanagemodule_setproperty
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certmod.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certidl.lib
 - Certidl.dll
api_name:
 - ICertManageModule.SetProperty
 - CCertManageModule.SetProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertManageModule::SetProperty


## -description


The <b>SetProperty</b> method allows a module to set a property value.


## -parameters




### -param strConfig [in]

Represents the configuration string for the Certificate Services server in the form COMPUTERNAME\CANAME, where COMPUTERNAME is the Certificate Services server's network name, and CANAME is the common name of the <a href="https://msdn.microsoft.com/en-us/library/ms721572(v=VS.85).aspx">certification authority</a> (CA) as entered for the CA during Certificate Services setup. For information about the configuration string name, see 
<a href="https://msdn.microsoft.com/en-us/library/Aa383268(v=VS.85).aspx">ICertConfig</a>.


### -param strStorageLocation [in]

The location that provides storage for the property values, as described in the definition of <i>strStorageLocation</i> in 
<a href="https://msdn.microsoft.com/en-us/library/Aa385031(v=VS.85).aspx">ICertManageModule::GetProperty</a>.


### -param strPropertyName [in]

The name of the property whose value is being assigned. Policy and exit modules should support the following properties, which are used by Certificate Services Manager.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="Name"></a><a id="name"></a><a id="NAME"></a><dl>
<dt><b>Name</b></dt>
</dl>
</td>
<td width="60%">
Name of the module.

</td>
</tr>
<tr>
<td width="40%"><a id="Description"></a><a id="description"></a><a id="DESCRIPTION"></a><dl>
<dt><b>Description</b></dt>
</dl>
</td>
<td width="60%">
Description of the module.

</td>
</tr>
<tr>
<td width="40%"><a id="Copyright"></a><a id="copyright"></a><a id="COPYRIGHT"></a><dl>
<dt><b>Copyright</b></dt>
</dl>
</td>
<td width="60%">
Copyright pertaining to the module.

</td>
</tr>
<tr>
<td width="40%"><a id="File_Version"></a><a id="file_version"></a><a id="FILE_VERSION"></a><dl>
<dt><b>File Version</b></dt>
</dl>
</td>
<td width="60%">
Version of the module file.

</td>
</tr>
<tr>
<td width="40%"><a id="Product_Version"></a><a id="product_version"></a><a id="PRODUCT_VERSION"></a><dl>
<dt><b>Product Version</b></dt>
</dl>
</td>
<td width="60%">
Version of the module.

</td>
</tr>
</table>
 


### -param Flags [in]

This parameter is reserved and must be set to zero.


### -param pvarProperty [in]

A value that is being assigned to the property specified by <i>strPropertyName</i>.


## -returns



<h3>VB</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.




## -remarks



This method is intended for future functionality. A minimal implementation is required, however, to meet the requirements of the <a href="https://msdn.microsoft.com/en-us/library/Aa385029(v=VS.85).aspx">ICertManageModule</a> interface.


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#include &lt;windows.h&gt;
#include &lt;Certmod.h&gt;

HRESULT CCertManagePolicyModule::SetProperty(
            /* [in] */ const BSTR strConfig,
            /* [in] */ BSTR strStorageLocation,
            /* [in] */ BSTR strPropertyName,
            /* [in] */ LONG Flags,
            /* [in] */ const VARIANT *pvarProperty)
{
    // This implementation fulfills the minimal requirement
    // needed for ICertManageModule::SetProperty.
    return S_OK;
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>CCertManageModule</b>



<a href="https://msdn.microsoft.com/en-us/library/Aa383268(v=VS.85).aspx">ICertConfig</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa385029(v=VS.85).aspx">ICertManageModule</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa385031(v=VS.85).aspx">ICertManageModule::GetProperty</a>
 

 

