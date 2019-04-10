---
UID: NF:wmsdkidl.IWMProfile.RemoveMutualExclusion
title: IWMProfile::RemoveMutualExclusion (wmsdkidl.h)
author: windows-sdk-content
description: The RemoveMutualExclusion method removes a mutual exclusion object from the profile.
old-location: wmformat\iwmprofile_removemutualexclusion.htm
tech.root: wmformat
ms.assetid: eb453285-a4e5-48dd-a4d0-72d2e09badc2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMProfile interface [windows Media Format],RemoveMutualExclusion method, IWMProfile.RemoveMutualExclusion, IWMProfile2 interface [windows Media Format],RemoveMutualExclusion method, IWMProfile2::RemoveMutualExclusion, IWMProfile3 interface [windows Media Format],RemoveMutualExclusion method, IWMProfile3::RemoveMutualExclusion, IWMProfile::RemoveMutualExclusion, IWMProfileRemoveMutualExclusion, RemoveMutualExclusion, RemoveMutualExclusion method [windows Media Format], RemoveMutualExclusion method [windows Media Format],IWMProfile interface, RemoveMutualExclusion method [windows Media Format],IWMProfile2 interface, RemoveMutualExclusion method [windows Media Format],IWMProfile3 interface, wmformat.iwmprofile_removemutualexclusion, wmsdkidl/IWMProfile2::RemoveMutualExclusion, wmsdkidl/IWMProfile3::RemoveMutualExclusion, wmsdkidl/IWMProfile::RemoveMutualExclusion
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 7 SDK, or later versions of the SDK
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmvcore.lib
 - Wmvcore.dll
 - WMStubDRM.lib
 - WMStubDRM.dll
 - qasf.dll
api_name:
 - IWMProfile.RemoveMutualExclusion
 - IWMProfile2.RemoveMutualExclusion
 - IWMProfile3.RemoveMutualExclusion
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMProfile::RemoveMutualExclusion


## -description



The <b>RemoveMutualExclusion</b> method removes a mutual exclusion object from the profile.




## -parameters




### -param pME [in]

Pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd757238(v=VS.85).aspx">IWMMutualExclusion</a> interface of the mutual exclusion object you want to remove.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>pcME</i> parameter is <b>NULL</b>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/00f28d6b-d27d-4268-960e-c8ea25e5359e">IWMProfile Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd757266(v=VS.85).aspx">IWMProfile2</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd757268(v=VS.85).aspx">IWMProfile3</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd757398(v=VS.85).aspx">IWMProfile::AddMutualExclusion</a>
 

 

