---
UID: NF:cluadmex.IWCWizardCallback.AddWizardPage
title: IWCWizardCallback::AddWizardPage
author: windows-sdk-content
description: Adds a property page to a Failover Cluster Administrator Wizard.
old-location: mscs\iwcwizardcallback_addwizardpage.htm
tech.root: mscs
ms.assetid: e5ce7798-c1e6-47b6-a1bf-1262b3511b22
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddWizardPage, AddWizardPage method [Failover Cluster], AddWizardPage method [Failover Cluster],IWCWizardCallback interface, IWCWizardCallback interface [Failover Cluster],AddWizardPage method, IWCWizardCallback.AddWizardPage, IWCWizardCallback::AddWizardPage, _wolf_iwcwizardcallback_addwizardpage, cluadmex/IWCWizardCallback::AddWizardPage, mscs.iwcwizardcallback_addwizardpage
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
 - IWCWizardCallback.AddWizardPage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWCWizardCallback::AddWizardPage


## -description


<p class="CCE_Message">[This method is available for use in the operating systems specified in the Requirements 
    section. Support for this method was removed in Windows Server 2008.]

Adds a property page to a Failover Cluster Administrator Wizard.


## -parameters




### -param hpage [in]

Handle to the property page to be added.


## -returns



If <b>AddWizardPage</b> is not successful, 
       it can return other <b>HRESULT</b> values.

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




<a href="https://msdn.microsoft.com/en-us/library/Aa369060(v=VS.85).aspx">Failover Cluster Administrator</a> extensions call the 
     <b>AddWizardPage</b> method from their 
     <a href="https://msdn.microsoft.com/en-us/library/Aa370738(v=VS.85).aspx">IWEExtendWizard::CreateWizardPages</a> 
     methods. Before calling <b>AddWizardPage</b>, 
     extensions must call the function 
     <a href="https://msdn.microsoft.com/en-us/library/Bb760807(v=VS.85).aspx">CreatePropertySheetPage</a> to retrieve a 
     handle to pass in the <i>hpage</i> parameter.

Use 
     <a href="https://msdn.microsoft.com/en-us/library/Aa370512(v=VS.85).aspx">IWCWizard97Calllback::AddWizard97Page</a> 
     to add Wizard97 pages.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa370512(v=VS.85).aspx">IWCWizard97Callback::AddWizard97Page</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa370517(v=VS.85).aspx">IWCWizardCallback</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa370738(v=VS.85).aspx">IWEExtendWizard::CreateWizardPages</a>
 

 

