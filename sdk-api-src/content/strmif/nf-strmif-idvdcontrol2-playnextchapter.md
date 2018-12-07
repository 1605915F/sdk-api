---
UID: NF:strmif.IDvdControl2.PlayNextChapter
title: IDvdControl2::PlayNextChapter
author: windows-sdk-content
description: The PlayNextChapter method starts playback from the beginning of the next chapter in the current title.
old-location: dshow\idvdcontrol2_playnextchapter.htm
tech.root: DirectShow
ms.assetid: 654841ce-6689-47cc-93fb-bd8de8f4dd3a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDvdControl2 interface [DirectShow],PlayNextChapter method, IDvdControl2.PlayNextChapter, IDvdControl2::PlayNextChapter, IDvdControl2PlayNextChapter, PlayNextChapter, PlayNextChapter method [DirectShow], PlayNextChapter method [DirectShow],IDvdControl2 interface, dshow.idvdcontrol2_playnextchapter, strmif/IDvdControl2::PlayNextChapter
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IDvdControl2.PlayNextChapter
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDvdControl2::PlayNextChapter


## -description



The <code>PlayNextChapter</code> method starts playback from the beginning of the next chapter in the current title.




## -parameters




### -param dwFlags [in]

Bitwise OR of one or more flags from the <a href="https://msdn.microsoft.com/05eb5ab8-a1b3-4876-bac3-29510af8cdbd">DVD_CMD_FLAGS</a> enumeration, specifying how to synchronize the command.


### -param ppCmd [out]

Receives a pointer to an <a href="https://msdn.microsoft.com/85f9b208-ddc2-4d9c-a30b-b666c81a49d2">IDvdCmd</a> object that can be used to synchronize DVD commands. The caller must release the interface. This parameter can be <b>NULL</b>. For more information, see <a href="https://msdn.microsoft.com/37e8f940-617d-43f6-92bd-aadccafe0059">Synchronizing DVD Commands</a>.


## -returns



Returns one of the following values.

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
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VFW_E_DVD_OPERATION_INHIBITED</b></dt>
</dl>
</td>
<td width="60%">
UOP control prohibits the operation.

</td>
</tr>
</table>
 




## -remarks



After playing the next chapter, the DVD Navigator continues playing, following the branching instructions on the disc. To play only the next chapter, call <a href="https://msdn.microsoft.com/fdf9642b-ac90-4ffc-a813-4a5b22a973dd">IDvdControl2::PlayChaptersAutoStop</a>.

This method is demonstrated in the DVDSample application in <b>CDvdCore::NextChapter</b>.

The following table shows the Annex J command name to which this method name corresponds, and the domains in which this method is valid.

<table>
<tr>
<td>Annex J Command Name
            </td>
<td>Valid Domains
            </td>
</tr>
<tr>
<td>NextPG_Search</td>
<td>
<ul>
<li>DVD_DOMAIN_VideoManagerMenu</li>
<li>DVD_DOMAIN_VideoTitleSetMenu</li>
<li>DVD_DOMAIN_Title</li>
</ul>
</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/6f41e0f1-e550-4ca6-9a80-ce4d498289e2">DVD Applications</a>



<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/eda43b20-1c4d-4769-bb87-3942716af13c">IDvdControl2 Interface</a>



<a href="https://msdn.microsoft.com/37e8f940-617d-43f6-92bd-aadccafe0059">Synchronizing DVD Commands</a>
 

 

