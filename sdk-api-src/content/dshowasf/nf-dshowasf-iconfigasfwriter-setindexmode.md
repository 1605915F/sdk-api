---
UID: NF:dshowasf.IConfigAsfWriter.SetIndexMode
title: IConfigAsfWriter::SetIndexMode (dshowasf.h)
author: windows-sdk-content
description: The SetIndexMode method controls whether the WM ASF Writer filter creates a file with a temporal index.
old-location: dshow\iconfigasfwriter_setindexmode.htm
tech.root: DirectShow
ms.assetid: d7f5d13a-d36e-4da2-babc-0446e5697b61
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IConfigAsfWriter interface [DirectShow],SetIndexMode method, IConfigAsfWriter.SetIndexMode, IConfigAsfWriter::SetIndexMode, IConfigAsfWriterSetIndexMode, SetIndexMode, SetIndexMode method [DirectShow], SetIndexMode method [DirectShow],IConfigAsfWriter interface, dshow.iconfigasfwriter_setindexmode, dshowasf/IConfigAsfWriter::SetIndexMode
ms.topic: method
req.header: dshowasf.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dshowasf.h
api_name:
 - IConfigAsfWriter.SetIndexMode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IConfigAsfWriter::SetIndexMode


## -description



The <code>SetIndexMode</code> method controls whether the WM ASF Writer filter creates a file with a temporal index.




## -parameters




### -param bIndexFile [in]

Specifies the index mode. If <b>TRUE</b>, the file will be indexed.


## -returns



Returns S_OK if successful, or an <b>HRESULT</b> error code otherwise.




## -remarks



By default, the WM ASF Writer filter creates temporally indexed ASF files. It performs the indexing when the graph stops. You can disable this behavior if you want to do your own frame-based indexing as a post-processing step. To create a frame-indexed file, call <code>SetIndexMode</code> with the value <b>FALSE</b>, create the file, and then use the Windows Media Format SDK methods to create a frame-based index for the file.




## -see-also




<a href="https://msdn.microsoft.com/dffda43a-5831-4889-864f-81351b9e2bb3">Creating ASF Files in DirectShow</a>



<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd312017(v=VS.85).aspx">IConfigAsfWriter Interface</a>
 

 

