---
UID: NN:vsmgmt.IVssSnapshotMgmt
title: IVssSnapshotMgmt (vsmgmt.h)
author: windows-sdk-content
description: Provides a method that returns an interface to further configure a shadow copy provider.
old-location: base\ivsssnapshotmgmt.htm
tech.root: VSS
ms.assetid: 5e5694a1-7c17-4d8a-b094-09dcf28a636f
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVssSnapshotMgmt, IVssSnapshotMgmt interface [Files], IVssSnapshotMgmt interface [Files],described, base.ivsssnapshotmgmt, vsmgmt/IVssSnapshotMgmt
ms.topic: interface
req.header: vsmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
 - VsMgmt.h
api_name:
 - IVssSnapshotMgmt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVssSnapshotMgmt interface


## -description


The <b>IVssSnapshotMgmt</b> interface provides a 
    method that returns an interface to further configure a shadow copy provider.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVssSnapshotMgmt</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IVssSnapshotMgmt</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVssSnapshotMgmt</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/814c6e2c-a5f8-4f44-b508-3a2e95bb1c54">GetProviderMgmtInterface</a>
</td>
<td align="left" width="63%">
Returns an interface to further configure a shadow copy provider.</p> (Inherited from <b>IVssSnapshotMgmt</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c74322d8-24a6-4463-82a5-c06e7624a1ca">QuerySnapshotsByVolume</a>
</td>
<td align="left" width="63%">
Reserved for system use.</p> (Inherited from <b>IVssSnapshotMgmt</b>)</td>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c3c4f0a1-eff5-4e83-8a1d-16e007bd119a">QueryVolumesSupportedForSnapshots</a>
</td>
<td align="left" width="63%">
Reserved for system use.</p> (Inherited from <b>IVssSnapshotMgmt</b>)</td>
</tr>
</table> 


## -remarks



The <b>IVssSnapshotMgmt</b> interface can be invoked 
    remotely using DCOM. The caller must be a member of the local administrators group on the remote machine.


#### Examples


```cpp
#include "vss.h"
#include "vsmgmt.h"

void main()
{
    // software-provider id is {b5946137-7b9f-4925-af80-51abd60b20d5}
    const VSS_ID ProviderId = { 0xb5946137, 
                                0x7b9f, 
                                0x4925, 
                              { 0xaf,0x80,0x51,0xab,0xd6,0xb,0x20,0xd5 } };

    HRESULT                               hr        = S_OK;
    IVssSnapshotMgmt*                     pMgmt     = NULL;
    IVssDifferentialSoftwareSnapshotMgmt* pDiffMgmt = NULL;

    hr = CoCreateInstance(CLSID_VssSnapshotMgmt,
                          NULL,
                          CLSCTX_ALL,
                          IID_IVssSnapshotMgmt,
                          (void**)&(pMgmt));
    if (FAILED(hr)) 
    {
        // error handling code
    }

    hr = pMgmt->GetProviderMgmtInterface(ProviderId, 
                                         IID_IVssDifferentialSoftwareSnapshotMgmt, 
                                         (IUnknown**)&pDiffMgmt);
    if (FAILED(hr)) 
    {
        pMgmt->Release();
    }

    // processing code

    pDiffMgmt->Release();
    pMgmt->Release();
}

```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a>



<a href="https://msdn.microsoft.com/3a0c60df-666c-4e33-a54c-7fa5ddbfde13">Volume Shadow Copy API Interfaces</a>
 

 

