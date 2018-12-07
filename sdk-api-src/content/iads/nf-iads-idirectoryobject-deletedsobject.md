---
UID: NF:iads.IDirectoryObject.DeleteDSObject
title: IDirectoryObject::DeleteDSObject
author: windows-sdk-content
description: Deletes a leaf object in a directory tree.
old-location: adsi\idirectoryobject_deletedsobject.htm
tech.root: adsi
ms.assetid: bb7bed74-1420-4b46-92a9-ebe31f2d88fd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DeleteDSObject, DeleteDSObject method [ADSI], DeleteDSObject method [ADSI],IDirectoryObject interface, IDirectoryObject interface [ADSI],DeleteDSObject method, IDirectoryObject.DeleteDSObject, IDirectoryObject::DeleteDSObject, _ds_idirectoryobject_deletedsobject, adsi.idirectoryobject__deletedsobject, adsi.idirectoryobject_deletedsobject, iads/IDirectoryObject::DeleteDSObject
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: iads.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Activeds.dll
api_name:
 - IDirectoryObject.DeleteDSObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirectoryObject::DeleteDSObject


## -description


The <b>IDirectoryObject::DeleteDSObject</b> method deletes a leaf object in a directory tree.


## -parameters




### -param pszRDNName

The relative distinguished name (relative path) of the object to be deleted.


## -returns



This method returns the standard return values, including S_OK for a successful operation. For more information and other return values, see  <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>.




## -remarks



To delete a container object and its children, use the  <a href="https://msdn.microsoft.com/53685f60-9adf-40f0-b6d3-e59a0435f744">IADsDeleteOps::DeleteObject</a> method.


#### Examples

The following C/C++ code example shows how to delete a user object.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>HRESULT hr;
IDirectoryObject *pDirObject=NULL;
hr = ADsGetObject(L"LDAP://OU=Sales,DC=Fabrikam,DC=com",
    IID_IDirectoryObject, (void**) &amp;pDirObject );
 
if ( SUCCEEDED(hr) )
{
    hr = pDirObject-&gt;DeleteDSObject( L"CN=Jeff Smith" );

    pDirObject-&gt;Release();
} 
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>



<a href="https://msdn.microsoft.com/53685f60-9adf-40f0-b6d3-e59a0435f744">IADsDeleteOps::DeleteObject</a>



<a href="https://msdn.microsoft.com/bc4f8920-2881-4393-bb01-ed837c3db6ad">IDirectoryObject</a>
 

 

