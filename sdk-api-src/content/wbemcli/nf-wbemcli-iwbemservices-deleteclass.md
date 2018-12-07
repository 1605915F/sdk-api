---
UID: NF:wbemcli.IWbemServices.DeleteClass
title: IWbemServices::DeleteClass
author: windows-sdk-content
description: The IWbemServices::DeleteClass method deletes the specified class from the current namespace.
old-location: wmi\iwbemservices_deleteclass.htm
tech.root: WmiSdk
ms.assetid: 1266d93a-776c-481d-b343-826a5c808d24
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DeleteClass, DeleteClass method [Windows Management Instrumentation], DeleteClass method [Windows Management Instrumentation],IWbemServices interface, IWbemServices interface [Windows Management Instrumentation],DeleteClass method, IWbemServices.DeleteClass, IWbemServices::DeleteClass, WBEM_FLAG_OWNER_UPDATE, WBEM_FLAG_RETURN_IMMEDIATELY, _hmm_iwbemservices_deleteclass, wbemcli/IWbemServices::DeleteClass, wmi.iwbemservices_deleteclass
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wbemcli.h
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
req.dll: Fastprox.dll; Esscli.dll; FrameDyn.dll; FrameDynOS.dll; Ntevt.dll; Stdprov.dll; Viewprov.dll; Wbemcomn.dll; Wbemcore.dll; Wbemess.dll; Wbemsvc.dll; Wmipicmp.dll; Wmidcprv.dll; Wmipjobj.dll; Wmiprvsd.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fastprox.dll
 - Esscli.dll
 - FrameDyn.dll
 - FrameDynOS.dll
 - Ntevt.dll
 - Stdprov.dll
 - Viewprov.dll
 - Wbemcomn.dll
 - Wbemcore.dll
 - Wbemess.dll
 - Wbemsvc.dll
 - Wmipicmp.dll
 - Wmidcprv.dll
 - Wmipjobj.dll
 - Wmiprvsd.dll
api_name:
 - IWbemServices.DeleteClass
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWbemServices::DeleteClass


## -description


The 
<b>IWbemServices::DeleteClass</b> method deletes the specified class from the current namespace. If a dynamic instance provider is associated with the class, the provider is unregistered, and it is no longer called for by that class. Any classes that derive from the deleted class are also deleted, and their associated providers are unregistered. All outstanding static instances of the specified class and its subclasses are also deleted when the class is deleted.

If a dynamic class provider provides the class, the success of the deletion depends on whether the provider supports class deletion.
<div class="alert"><b>Note</b>  System classes cannot be deleted.</div><div> </div>

## -parameters




### -param strClass [in]

Name of the class targeted for deletion.


### -param lFlags [in]

One of the following values can be set.



#### WBEM_FLAG_RETURN_IMMEDIATELY

This flag causes this to be a semisynchronous call. For more information, see 
<a href="https://msdn.microsoft.com/7a1eda93-014e-4067-b6d0-361a3d2fd1df">Calling a Method</a>.



#### WBEM_FLAG_OWNER_UPDATE

Indicates that the caller is a push provider.


### -param pCtx [in]

Typically <b>NULL</b>. Otherwise, this is a pointer to an 
<a href="https://msdn.microsoft.com/458bd455-6984-414b-a0b7-62887d9dad7c">IWbemContext</a> object that may be used by the provider deleting the class. The values in the context object must be specified in the documentation for the provider in question. For more information about this parameter, see 
<a href="https://msdn.microsoft.com/5bfd9d9b-ffe5-4def-a97d-85c4c01223f0">Making Calls to WMI</a>.


### -param ppCallResult [out]

If <b>NULL</b>, this parameter is not used. If <i>ppCallResult</i> is specified, it must be set to point to <b>NULL</b> on entry. If the <i>lFlags</i> parameter contains <b>WBEM_FLAG_RETURN_IMMEDIATELY</b>, this call returns immediately with <b>WBEM_S_NO_ERROR</b>. The <i>ppCallResult</i> parameter receives a pointer to a new 
<a href="https://msdn.microsoft.com/f0aa0233-3b9b-4757-bfdc-26d9fd556ce9">IWbemCallResult</a> object, which can then be polled to obtain the result using the 
<a href="https://msdn.microsoft.com/5a600fd8-87d8-446d-93da-5b22fd575a11">GetCallStatus</a> method.


## -returns



This method returns an <b>HRESULT</b> indicating the status of the method call. The following list lists the value contained withinan <b>HRESULT</b>.

On failure, you can obtain any available information from the COM function <a href="https://msdn.microsoft.com/03317526-8c4f-4173-bc10-110c8112676a">GetErrorInfo</a>.

COM-specific error codes may also be returned if network problems cause you to lose the remote connection to Windows Management.




## -see-also




<a href="https://msdn.microsoft.com/58e2ecca-7d1f-4831-93fc-f946f8ada2c0">IWbemServices</a>



<a href="https://msdn.microsoft.com/ebb58f3b-201c-4e37-8a51-9b5e2365cf3c">IWbemServices::DeleteClassAsync</a>



<a href="https://msdn.microsoft.com/f54b8e7c-c531-47d5-bab8-780652b94555">Retrieving an Error Code</a>
 

 

