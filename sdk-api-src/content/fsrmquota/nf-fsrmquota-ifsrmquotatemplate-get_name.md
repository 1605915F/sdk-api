---
UID: NF:fsrmquota.IFsrmQuotaTemplate.get_Name
title: IFsrmQuotaTemplate::get_Name (fsrmquota.h)
author: windows-sdk-content
description: Retrieves and sets the name of the quota template.
old-location: fsrm\ifsrmquotatemplate_name.htm
tech.root: fsrm
ms.assetid: 77a38b03-eb47-4298-ac13-44ffbd649752
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IFsrmQuotaTemplate interface [File Server Resource Manager],Name property, IFsrmQuotaTemplate.Name, IFsrmQuotaTemplate.get_Name, IFsrmQuotaTemplate::Name, IFsrmQuotaTemplate::get_Name, IFsrmQuotaTemplate::put_Name, Name property [File Server Resource Manager], Name property [File Server Resource Manager],IFsrmQuotaTemplate interface, fs.ifsrmquotatemplate_name, fsrm.ifsrmquotatemplate_name, fsrmquota/IFsrmQuotaTemplate::Name, fsrmquota/IFsrmQuotaTemplate::get_Name, fsrmquota/IFsrmQuotaTemplate::put_Name, get_Name
ms.topic: method
req.header: fsrmquota.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.dll: SrmSvc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - SrmSvc.dll
api_name:
 - IFsrmQuotaTemplate.Name
 - IFsrmQuotaTemplate.get_Name
 - IFsrmQuotaTemplate.put_Name
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFsrmQuotaTemplate::get_Name


## -description


<p class="CCE_Message">[This property is supported for compatibility but it's recommended to use the 
    <a href="https://msdn.microsoft.com/1CE772FA-CE33-4900-A499-058175A7C37E">FSRM WMI Classes</a> to manage FSRM. Please see the 
    <a href="https://msdn.microsoft.com/9308f1de-ba8e-45f5-81ec-d8203839ee79">MSFT_FSRMQuota</a> class.]

Retrieves and sets the name of the quota template.

This property is read/write.


## -parameters


## -remarks



If you do not specify a name, FSRM generates a unique name that begins with 
    "QuotaTemplate".


#### Examples

For an example, see <a href="https://msdn.microsoft.com/88ff3968-cb83-4b66-83e9-a58205b4be82">Using Templates to Define Quotas</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/de8ac383-f309-4320-bc77-c859ba27e1ca">IFsrmQuotaTemplate</a>



<a href="https://msdn.microsoft.com/9308f1de-ba8e-45f5-81ec-d8203839ee79">MSFT_FSRMQuota</a>
 

 

