---
UID: NF:strmif.IDvdControl.TopPGSearch
title: IDvdControl::TopPGSearch (strmif.h)
author: windows-sdk-content
description: Note  The IDvdControl interface is deprecated. Use IDvdControl2 instread. Halts playback of the current program and restarts playback of the current program within the program chain (PGC).
old-location: dshow\idvdcontrol_toppgsearch.htm
tech.root: DirectShow
ms.assetid: 35a621de-5110-4999-8475-ae84a4dc9ee1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IDvdControl interface [DirectShow],TopPGSearch method, IDvdControl.TopPGSearch, IDvdControl::TopPGSearch, IDvdControlTopPGSearch, TopPGSearch, TopPGSearch method [DirectShow], TopPGSearch method [DirectShow],IDvdControl interface, dshow.idvdcontrol_toppgsearch, strmif/IDvdControl::TopPGSearch
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - Strmif.h
api_name:
 - IDvdControl.TopPGSearch
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDvdControl::TopPGSearch


## -description



<div class="alert"><b>Note</b>  The <b>IDvdControl</b> interface is deprecated. Use <a href="https://msdn.microsoft.com/eda43b20-1c4d-4769-bb87-3942716af13c">IDvdControl2</a> instread.</div>
<div> </div>
Halts playback of the current program and restarts playback of the current program within the program chain (PGC).




## -parameters






## -returns



Returns an <b>HRESULT</b> value .




## -remarks



A program is usually equivalent to a chapter, and a PGC is usually equivalent to a title. In the case of One_Sequential_PGC_Titles, each program is required to be a chapter and each title has only one PGC, but in other cases (especially with random/shuffle PGCs and parental blocks) there can be more than one program between chapters and there can be more than one PGC in a title.

This method returns an error unless the domain is DVD_DOMAIN_VideoManagerMenu, DVD_DOMAIN_VideoTitleSetMenu, or DVD_DOMAIN_Title. For more information, see <a href="https://msdn.microsoft.com/2763a159-d4de-44c2-905b-5828f328cbd2">DVD_DOMAIN</a>.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/a6ca0fe8-84e3-43e6-9421-29dcff056dfd">IDvdControl Interface</a>
 

 

