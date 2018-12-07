---
UID: NF:cluadmex.IWCWizardCallback.EnableNext
title: IWCWizardCallback::EnableNext
author: windows-sdk-content
description: Enables or disables the Next or Finish button on a Failover Cluster Administrator Wizard page, depending on whether the current page is last.
old-location: mscs\iwcwizardcallback_enablenext.htm
tech.root: mscs
ms.assetid: 6f485ffa-0e94-4443-9c79-991c35a60e97
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnableNext, EnableNext method [Failover Cluster], EnableNext method [Failover Cluster],IWCWizardCallback interface, IWCWizardCallback interface [Failover Cluster],EnableNext method, IWCWizardCallback.EnableNext, IWCWizardCallback::EnableNext, _wolf_iwcwizardcallback_enablenext, cluadmex/IWCWizardCallback::EnableNext, mscs.iwcwizardcallback_enablenext
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: cluadmex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2003 Enterprise, Windows Server 2003 Datacenter
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: CluAdmEx.idl
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
 - cluadmex.h
api_name:
 - IWCWizardCallback.EnableNext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWCWizardCallback::EnableNext


## -description


<p class="CCE_Message">[This method is available for use in the operating systems specified in the Requirements 
    section. Support for this method was removed in Windows Server 2008.]

Enables or disables the <b>Next</b> or <b>Finish</b> button on a 
    Failover Cluster Administrator Wizard page, depending on whether the current page is last.


## -parameters




### -param hpage [in]

Handle to the property page containing the button to be enabled or disabled.


### -param bEnable [in]

Value indicating whether to enable or disable the button. If <i>bEnable</i> is set to 
       <b>TRUE</b>, the appropriate button is enabled. If <i>bEnable</i> is set 
       to <b>FALSE</b>, it is disabled.


## -returns



If <b>EnableNext</b> is not successful, it 
       can return other <b>HRESULT</b> values.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>NOERROR</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The operation was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
<dt>0x80070057</dt>
</dl>
</td>
<td width="60%">
The <i>hpage</i> parameter represents an unknown page.

</td>
</tr>
</table>
 




## -remarks



Extensions should call the <b>EnableNext</b> 
     method in their handling of the <b>PSN_SETACTIVE</b> message for a property page that 
     they have added to the Failover Cluster Administrator Wizard. 
     <a href="https://msdn.microsoft.com/en-us/library/Aa369060(v=VS.85).aspx">Failover Cluster Administrator</a> determines whether 
     the <b>Next</b> or <b>Finish</b> button should be displayed based on 
     the page specified in the <i>hpage</i> parameter.

For Wizard97 pages, use 
     <a href="https://msdn.microsoft.com/en-us/library/Aa370515(v=VS.85).aspx">IWCWizard97Callback::EnableNext</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa370515(v=VS.85).aspx">IWCWizard97Callback::EnableNext</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa370517(v=VS.85).aspx">IWCWizardCallback</a>
 

 

