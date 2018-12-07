---
UID: NF:control.IQueueCommand.InvokeAtStreamTime
title: IQueueCommand::InvokeAtStreamTime
author: windows-sdk-content
description: The InvokeAtStreamTime method queues a method or property change for execution at a specified stream time (that is, presentation time relative to the current stream time offset).
old-location: dshow\iqueuecommand_invokeatstreamtime.htm
tech.root: DirectShow
ms.assetid: 350b6842-207c-47db-a3f8-9e2784d9da67
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IQueueCommand interface [DirectShow],InvokeAtStreamTime method, IQueueCommand.InvokeAtStreamTime, IQueueCommand::InvokeAtStreamTime, IQueueCommandInvokeAtStreamTime, InvokeAtStreamTime, InvokeAtStreamTime method [DirectShow], InvokeAtStreamTime method [DirectShow],IQueueCommand interface, control/IQueueCommand::InvokeAtStreamTime, dshow.iqueuecommand_invokeatstreamtime
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: control.h
req.include-header: Dshow.h
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
 - IQueueCommand.InvokeAtStreamTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IQueueCommand::InvokeAtStreamTime


## -description



The <code>InvokeAtStreamTime</code> method queues a method or property change for execution at a specified stream time (that is, presentation time relative to the current stream time offset).




## -parameters




### -param pCmd [out]

Address of a variable that receives an <a href="https://msdn.microsoft.com/en-us/library/Dd406762(v=VS.85).aspx">IDeferredCommand</a> interface pointer.


### -param time [in]

Time at which to invoke the command.


### -param iid [in]

Pointer to the interface identifier (IID) of interface.


### -param dispidMethod [in]

Dispatch identifier (DISPID) of a method or property on the interface. Equivalent to the <i>dispIdMember</i> parameter of the <b>IDispatch::Invoke</b> method.


### -param wFlags [in]

Flags describing the context of the call. Equivalent to the <i>wFlags</i> parameter of the <b>IDispatch::Invoke</b> method.


### -param cArgs [in]

Number of arguments in <i>pDispParams</i>. Equivalent to the <b>cArgs</b> member of the <b>DISPPARAMS</b> structure.


### -param pDispParams [in]

Pointer to an array that contains the arguments. Equivalent to the <b>rgvarg</b> member of the <b>DISPPARAMS</b> structure.


### -param pvarResult [in, out]

Pointer to a VARIANT that receives the result. Equivalent to the <i>pVarResult</i> parameter of the <b>IDispatch::Invoke</b> method.


### -param puArgErr [out]

Pointer to a variable that receives the index of the first argument that has an error. Equivalent to the <i>puArgErr</i> parameter of the <b>IDispatch::Invoke</b> method.


## -returns



Returns an <b>HRESULT</b> value.




## -remarks



Use the <b>IDispatch::GetIDsOfNames</b> method to retrieve the DISPID for the <i>dispidMember</i> parameter.


#### Examples

The following example queues an <a href="https://msdn.microsoft.com/en-us/library/Dd390178(v=VS.85).aspx">IMediaControl::Stop</a> command for 3.0 seconds.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
IQueueCommand *pQ = 0;
IMediaControl *pControl = 0;

// Query for IQueueCommand.
pGraph-&gt;QueryInterface(IID_IQueueCommand, reinterpret_cast&lt;void**&gt;(&amp;pQ));

// Query for IMediaControl.
pGraph-&gt;QueryInterface(IID_IMediaControl, reinterpret_cast&lt;void**&gt;(&amp;pControl));

// Find the DISPID of the IMediaControl::Stop method.
OLECHAR *szMethod = OLESTR("Stop");

long dispid;
hr = pControl-&gt;GetIDsOfNames(IID_NULL, &amp;szMethod, 1, 0, &amp;dispid);

// Invoke the command.
IDeferredCommand *pCmd = 0;
hr = pQ-&gt;InvokeAtPresentationTime(&amp;pCmd, 3.0,
    const_cast&lt;GUID*&gt;(&amp;IID_IMediaControl), dispid, DISPATCH_METHOD, 
    0, 0, 0, 0);
if (SUCCEEDED(hr))
{
    pControl-&gt;Run();
    pCmd-&gt;Release();
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd375623(v=VS.85).aspx">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376922(v=VS.85).aspx">IQueueCommand Interface</a>
 

 

