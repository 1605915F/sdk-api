---
UID: NF:wbemprov.IWbemEventSink.SetSinkSecurity
title: IWbemEventSink::SetSinkSecurity
author: windows-sdk-content
description: Used to set a security descriptor (SD) on a sink for all the events passing through.
old-location: wmi\iwbemeventsink_setsinksecurity.htm
tech.root: WmiSdk
ms.assetid: 887b3c21-2ff6-4ae9-80bf-19f601da5e8b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWbemEventSink interface [Windows Management Instrumentation],SetSinkSecurity method, IWbemEventSink.SetSinkSecurity, IWbemEventSink::SetSinkSecurity, SetSinkSecurity, SetSinkSecurity method [Windows Management Instrumentation], SetSinkSecurity method [Windows Management Instrumentation],IWbemEventSink interface, _hmm_iwbemeventsink_setsinksecurity, wbemprov/IWbemEventSink::SetSinkSecurity, wmi.iwbemeventsink_setsinksecurity
ms.topic: method
req.header: wbemprov.h
req.include-header: Wbemidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
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
req.lib: Wbemuuid.lib
req.dll: Wbemsvc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wbemsvc.dll
api_name:
 - IWbemEventSink.SetSinkSecurity
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWbemEventSink::SetSinkSecurity


## -description


The 
<b>IWbemEventSink::SetSinkSecurity</b> method is used to set a security descriptor (SD) on a sink for all the events passing through. WMI handles the access checks based on the SD.  Use  this method when the provider cannot control what users are allowed to consume its events, but can set an SD for a specific sink.


## -parameters




### -param lSDLength [in]

Length of security descriptor.


### -param pSD [in]

Security descriptor, DACL.


## -returns



This method returns an <b>HRESULT</b> indicating the status of the method call. The following list lists the value contained within an <b>HRESULT</b>.




## -remarks



The SD DACL defines who has access to the events. The access control entry (ACE) of a consumer seeking access to the events delivered to the sink must match an ACE with <b>WBEM_RIGHT_SUBSCRIBE</b> set in the <i>pSD</i> parameter. The SD owner and group specify the identity to be used when raising the event. This identity can be different than the identity of the account raising the event; however, when checking access of the event against a filter SD, both the identity of the user and the identity specified in the owner field are checked for access. For more information, see the <b>EventAccess</b> property of the 
<a href="https://msdn.microsoft.com/369d3c28-2b69-456f-9144-d7c73e3123bc">__EventFilter</a> class. The group field of the SD must be set and the SACL field is not used.  For more information about event security and when to use this method, see <a href="https://msdn.microsoft.com/86eaeb5c-c27e-4794-88e2-e0ffbb885290">Securing WMI Events</a>.

For more information about providing events, see <a href="https://msdn.microsoft.com/075bdc65-4ea3-4f91-9823-1d2d0dc13423">Writing an Event Provider</a>.


#### Examples

The following code example sets the SD for all the events provided through the sink.The code requires the following #include statements and references.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#define _WIN32_WINNT 0x0500
#define SECURITY_WIN32
#pragma comment(lib, "wbemuuid.lib")
#pragma comment(lib, "Secur32.lib")
#include &lt;windows.h&gt;
#include &lt;sddl.h&gt;
#include &lt;wbemidl.h&gt;
#include &lt;security.h&gt;
#include &lt;iostream&gt;
using namespace std;

HRESULT CMyEventProvider::ProvideEvents( IWbemObjectSink *pSink,
                                            long lFlags )
{
    IWbemEventSink *pEventSink = NULL;
    //Create SD with allowing only administrators
    // to receive events. O:BAG:BAD:(A;;0x40;;;BA)
     long lMask = WBEM_RIGHT_SUBSCRIBE;
     WCHAR wBuf[MAX_PATH];
     _ltow( lMask, wBuf, 16 );
 
       wstring wstrSD = L"O:BAG:BAD:(A;;0x";
        wstrSD += lMask;
       wstrSD += L";;;BA)";
    ULONG ulSize = 0;
    PSECURITY_DESCRIPTOR pSD = NULL;
 
    ConvertStringSecurityDescriptorToSecurityDescriptorW(
        wstrSD.c_str(), SDDL_REVISION_1, &amp;pSD, &amp;ulSize ); 
    HRESULT hRes = pSink-&gt;QueryInterface( IID_IWbemEventSink,
        (void**)pEventSink );
    if( SUCCEEDED(hRes) )
        hRes = pEventSink-&gt;SetSinkSecurity( ulLength, pSD );
    LocalFree(pSD );
    return hRes;
}</pre>
</td>
</tr>
</table></span></div>


