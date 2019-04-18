---
UID: NF:wmsdkidl.IWMProfile.CreateNewMutualExclusion
title: IWMProfile::CreateNewMutualExclusion (wmsdkidl.h)
author: windows-sdk-content
description: The CreateNewMutualExclusion method creates a mutual exclusion object. Mutual exclusion objects are used to specify a set of streams, only one of which can be output at a time.
old-location: wmformat\iwmprofile_createnewmutualexclusion.htm
tech.root: wmformat
ms.assetid: fcf3a549-5ae1-459a-95b9-923570f59a4a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CreateNewMutualExclusion, CreateNewMutualExclusion method [windows Media Format], CreateNewMutualExclusion method [windows Media Format],IWMProfile interface, CreateNewMutualExclusion method [windows Media Format],IWMProfile2 interface, CreateNewMutualExclusion method [windows Media Format],IWMProfile3 interface, IWMProfile interface [windows Media Format],CreateNewMutualExclusion method, IWMProfile.CreateNewMutualExclusion, IWMProfile2 interface [windows Media Format],CreateNewMutualExclusion method, IWMProfile2::CreateNewMutualExclusion, IWMProfile3 interface [windows Media Format],CreateNewMutualExclusion method, IWMProfile3::CreateNewMutualExclusion, IWMProfile::CreateNewMutualExclusion, IWMProfileCreateNewMutualExclusion, wmformat.iwmprofile_createnewmutualexclusion, wmsdkidl/IWMProfile2::CreateNewMutualExclusion, wmsdkidl/IWMProfile3::CreateNewMutualExclusion, wmsdkidl/IWMProfile::CreateNewMutualExclusion
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
 - IWMProfile.CreateNewMutualExclusion
 - IWMProfile2.CreateNewMutualExclusion
 - IWMProfile3.CreateNewMutualExclusion
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMProfile::CreateNewMutualExclusion


## -description



The <b>CreateNewMutualExclusion</b> method creates a mutual exclusion object. Mutual exclusion objects are used to specify a set of streams, only one of which can be output at a time.




## -parameters




### -param ppME [out]

Pointer to a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd757238(v=VS.85).aspx">IWMMutualExclusion</a> interface of the new mutual exclusion object.


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
The <i>ppME</i> parameter is <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



This creation method is included as a method to this interface, rather than as an independent function. For clarity, it is not possible to have a mutual exclusion object other than as an element of a profile.

After the application has created the mutual exclusion object, it must be configured and then <a href="https://msdn.microsoft.com/en-us/library/Dd757398(v=VS.85).aspx">AddMutualExclusion</a> must be called to add the mutual exclusion to the profile.




## -see-also




<a href="https://msdn.microsoft.com/00f28d6b-d27d-4268-960e-c8ea25e5359e">IWMProfile Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd757266(v=VS.85).aspx">IWMProfile2</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd757268(v=VS.85).aspx">IWMProfile3</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd757398(v=VS.85).aspx">IWMProfile::AddMutualExclusion</a>
 

 

