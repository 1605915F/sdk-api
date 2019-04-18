---
UID: NF:appxpackaging.IAppxManifestResourcesEnumerator.GetCurrent
title: IAppxManifestResourcesEnumerator::GetCurrent (appxpackaging.h)
author: windows-sdk-content
description: Gets the resource at the current position of the enumerator.
old-location: appxpkg\iappxmanifestresourcesenumerator_getcurrent.htm
tech.root: appxpkg
ms.assetid: FCFEEC2B-F047-4417-B110-BD3C90C30BE2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetCurrent, GetCurrent method [App packaging and management], GetCurrent method [App packaging and management],IAppxManifestResourcesEnumerator interface, IAppxManifestResourcesEnumerator interface [App packaging and management],GetCurrent method, IAppxManifestResourcesEnumerator.GetCurrent, IAppxManifestResourcesEnumerator::GetCurrent, appxpackaging/IAppxManifestResourcesEnumerator::GetCurrent, appxpkg.iappxmanifestresourcesenumerator_getcurrent
ms.topic: method
req.header: appxpackaging.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: AppxPackaging.idl
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
 - AppxPackaging.h
api_name:
 - IAppxManifestResourcesEnumerator.GetCurrent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAppxManifestResourcesEnumerator::GetCurrent


## -description


Gets the resource at the current position of the enumerator.


## -parameters




### -param resource [out, retval]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPWSTR</a>*</b>

The current resource.


## -returns



Type: <b>HRESULT</b>

If the method succeeds, it returns <b>S_OK</b>. Otherwise, it returns an error code that includes, but is not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_BOUNDS</b></dt>
</dl>
</td>
<td width="60%">
The enumerator has passed the last item in the collection.

</td>
</tr>
</table>
 




## -remarks



The caller must free the memory allocated for <i>resource</i> using the <a href="https://msdn.microsoft.com/3d0af12e-fc74-4ef7-b2dd-e9da5d0483c7">CoTaskMemFree</a> function.

The enumerator returned can be empty. In this case, a call to  <a href="https://msdn.microsoft.com/72798FDF-3296-4AC7-9BA0-212457F9BEC7">GetHasCurrent</a> returns <b>false</b>. If the enumerator is not empty, it points to the first element, and this method returns the first item. Subsequently, the user should use <a href="https://msdn.microsoft.com/CD5A7FF9-A28E-4857-AE7B-92F8EEBA0235">MoveNext</a> to move through the items, and call <b>GetHasCurrent</b> before using <b>GetCurrent</b> to access the item.




## -see-also




<a href="https://msdn.microsoft.com/D76C7512-962F-4AFE-934F-BBC215B5FE99">IAppxManifestResourcesEnumerator</a>
 

 

