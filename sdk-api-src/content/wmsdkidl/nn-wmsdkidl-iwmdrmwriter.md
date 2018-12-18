---
UID: NN:wmsdkidl.IWMDRMWriter
title: IWMDRMWriter
author: windows-sdk-content
description: The IWMDRMWriter interface provides support for applying DRM protection to content in ASF files.
old-location: wmformat\iwmdrmwriter.htm
tech.root: wmformat
ms.assetid: fd466cf8-b1f8-49aa-a486-8fd347b29178
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMDRMWriter, IWMDRMWriter interface [windows Media Format], IWMDRMWriter interface [windows Media Format],described, IWMDRMWriterInterface, wmformat.iwmdrmwriter, wmsdkidl/IWMDRMWriter
ms.topic: interface
req.header: wmsdkidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmsdkidl.h
api_name:
 - IWMDRMWriter
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDRMWriter interface


## -description


<p class="CCE_Message">[<b>IWMDRMWriter</b> is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. Instead, use <a href="http://go.microsoft.com/fwlink/p/?linkid=325240">Microsoft PlayReady</a>.
]


The <b>IWMDRMWriter</b> interface provides support for applying DRM protection to content in ASF files. You can use this interface to set various DRM file attributes and run-time properties, and to generate <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">DRM</a> keys for encrypting the content and the DRM header, without needing to call functions external to the Windows Media Format SDK. Prior to Windows Media 9 Series, it was necessary to use the Windows Media Rights Manager SDK to apply protection to files. The ability to protect files "on the fly" as you write them enables scenarios such as "Live DRM" in which live streaming content, such as a pay-per-view sports event or concert, can be delivered over the Internet.

An <b>IWMDRMWriter</b> interface exists for every writer object. You can obtain a pointer to an instance of this interface by calling the <b>QueryInterface</b> method of any interface in a writer object.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMDRMWriter</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMDRMWriter</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMDRMWriter</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd798377(v=VS.85).aspx">GenerateKeyID</a>
</td>
<td align="left" width="63%">
Generates a DRM <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">key ID</a> that will be used in conjunction with a key seed to encrypt and decrypt files.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd798378(v=VS.85).aspx">GenerateKeySeed</a>
</td>
<td align="left" width="63%">
Generates a DRM key seed that will be used in conjunction with a key ID to create protected files.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd798500(v=VS.85).aspx">GenerateSigningKeyPair</a>
</td>
<td align="left" width="63%">
Generates a public and a private key that will be used to sign the ASF header object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd798501(v=VS.85).aspx">SetDRMAttribute</a>
</td>
<td align="left" width="63%">
Sets DRM header attributes as well as other DRM run-time properties.

</td>
</tr>
</table> 

For information on other interfaces that can be obtained by using the QueryInterface method of this interface, see <a href="https://msdn.microsoft.com/8058b7fe-7d02-4572-ad43-6867d4ceb7e9">Writer Object</a>.



## -see-also




<a href="https://msdn.microsoft.com/222ef91c-b776-4de8-b1ad-88c2beca05aa">DRM Attribute List</a>



<a href="https://msdn.microsoft.com/862fc8bc-6e40-4496-862a-c12c8a382116">DRM Properties</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798373(v=VS.85).aspx">IWMDRMWriter2 Interface</a>



<a href="https://msdn.microsoft.com/c61a0739-09f2-497f-a2cd-d3f2472738e3">Interfaces</a>



<a href="https://msdn.microsoft.com/8058b7fe-7d02-4572-ad43-6867d4ceb7e9">Writer Object</a>
 

 

