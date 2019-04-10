---
UID: NC:userenv.PFNPROCESSGROUPPOLICYEX
title: PFNPROCESSGROUPPOLICYEX (userenv.h)
author: windows-sdk-content
description: The ProcessGroupPolicyEx function is an application-defined callback function used when applying policy.
old-location: policy\processgrouppolicyex.htm
tech.root: Policy
ms.assetid: df77fece-6e81-4a85-847a-fef3ba775e93
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GPO_INFO_FLAG_ASYNC_FOREGROUND, GPO_INFO_FLAG_BACKGROUND, GPO_INFO_FLAG_FORCED_REFRESH, GPO_INFO_FLAG_LINKTRANSITION, GPO_INFO_FLAG_LOGRSOP_TRANSITION, GPO_INFO_FLAG_MACHINE, GPO_INFO_FLAG_NOCHANGES, GPO_INFO_FLAG_SAFEMODE_BOOT, GPO_INFO_FLAG_SLOWLINK, GPO_INFO_FLAG_VERBOSE, PFNPROCESSGROUPPOLICYEX, PFNPROCESSGROUPPOLICYEX callback, PFNPROCESSGROUPPOLICYEX callback function [Group Policy], ProcessGroupPolicyEx, _win32_processgrouppolicyex, policy.processgrouppolicyex, userenv/PFNPROCESSGROUPPOLICYEX
ms.topic: callback
req.header: userenv.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Userenv.h
api_name:
 - PFNPROCESSGROUPPOLICYEX
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFNPROCESSGROUPPOLICYEX callback function


## -description


The <b>ProcessGroupPolicyEx</b> function is an 
  application-defined callback function used when applying policy. This extended function also supports the logging of 
  Resultant Set of Policy (RSoP) data. The <b>PFNPROCESSGROUPPOLICYEX</b> type defines a pointer 
  to this callback function. <b>ProcessGroupPolicyEx</b> 
  is a placeholder for the application-defined function name.


## -parameters




### -param dwFlags [in]

This parameter can be one or more of the following flags.



#### GPO_INFO_FLAG_MACHINE

Apply computer policy rather than user policy.



#### GPO_INFO_FLAG_BACKGROUND

Perform a background refresh of the policy. For more information, see the text following this list.



#### GPO_INFO_FLAG_ASYNC_FOREGROUND

Perform an asynchronous foreground refresh of policy. For more information, see the text following this 
        list. For more information about foreground policy application, see 
        <a href="https://msdn.microsoft.com/60774d80-32a0-446e-b394-a45a9aaf6325">Initial Processing of Group Policy</a>.



#### GPO_INFO_FLAG_SLOWLINK

The policy is being applied across a slow link.



#### GPO_INFO_FLAG_VERBOSE

Write verbose output to the event log.



#### GPO_INFO_FLAG_NOCHANGES

No changes to the GPO were detected.



#### GPO_INFO_FLAG_LINKTRANSITION

A change in the link speed was detected between policy applications.



#### GPO_INFO_FLAG_LOGRSOP_TRANSITION

A change in RSoP logging was detected between the application of the previous policy and the application 
        of the current policy.



#### GPO_INFO_FLAG_FORCED_REFRESH

A forced policy refresh is being applied.



#### GPO_INFO_FLAG_SAFEMODE_BOOT

Safe mode flag.

The <b>GPO_INFO_FLAG_BACKGROUND</b> flag and the 
       <b>GPO_INFO_FLAG_ASYNC_FOREGROUND</b> flag can both be set. Because policies are always applied asynchronously during a 
<a href="https://msdn.microsoft.com/fb585a05-50a9-48c5-b6b0-c488dad4849f">background refresh</a>, most extensions handle an asynchronous foreground refresh in the same manner in which they handle a background refresh. Therefore, they do not need to check for the <b>GPO_INFO_FLAG_ASYNC_FOREGROUND</b> flag. In instances when an extension must distinguish between a background refresh of policy and an asynchronous foreground refresh of policy, the extension can check for the <b>GPO_INFO_FLAG_ASYNC_FOREGROUND</b> flag.


### -param hToken [in]

Token for the user or computer, returned from the 
<a href="https://msdn.microsoft.com/a6d880a0-0aed-4bdb-89c9-4f667ecb510e">LogonUser</a>, 
<a href="https://msdn.microsoft.com/e087f360-5d1d-4846-b3d6-214a426e5222">CreateRestrictedToken</a>, 
<a href="https://msdn.microsoft.com/796ec60e-fcae-48a9-b471-de3dce831306">DuplicateToken</a>, 
<a href="https://msdn.microsoft.com/1e760ad8-7e46-4748-8c45-36ad8efe936a">OpenProcessToken</a>, or 
<a href="https://msdn.microsoft.com/5003f0c4-41e9-4a14-b6a9-4f259c4af08b">OpenThreadToken</a> function. This token must have <b>TOKEN_IMPERSONATE</b> and <b>TOKEN_QUERY</b> access. For more information, see 
<a href="https://msdn.microsoft.com/5f710fd8-33de-47c0-a8b2-baf3008c4ed7">Access Rights for Access-Token Objects</a> and 
<a href="https://msdn.microsoft.com/a3f74372-bdc9-43eb-b72f-7d00a43e78a8">Client Impersonation</a>.


### -param hKeyRoot [in]

Handle to the <b>HKEY_LOCAL_MACHINE</b> or <b>HKEY_CURRENT_USER</b> registry key.


### -param pDeletedGPOList [in]

Pointer that receives the list of deleted GPO structures. For more information, see 
<a href="https://msdn.microsoft.com/7275a3cd-6b19-4eb9-9481-b73bd5af5753">GROUP_POLICY_OBJECT</a>.


### -param pChangedGPOList [in]

Pointer that receives the list of changed GPO structures. For more information, see 
<a href="https://msdn.microsoft.com/7275a3cd-6b19-4eb9-9481-b73bd5af5753">GROUP_POLICY_OBJECT</a>.


### -param pHandle [in]

Asynchronous completion handle. If the callback function does not support asynchronous processing, this handle is zero.


### -param *pbAbort [in]

Specifies whether to continue processing GPOs. If this parameter is <b>TRUE</b>, GPO processing will cease. If this parameter is <b>FALSE</b>, GPO processing will continue.


### -param pStatusCallback [in]

Pointer to a 
<a href="https://msdn.microsoft.com/9eec6204-49b5-49fd-8db4-5c1777eb7c85">StatusMessageCallback</a> callback function that displays status messages. This parameter can be <b>NULL</b> in certain cases. For example, if the system is applying policy in the background, the status user interface is not present and the application cannot send status messages to be displayed. For more information, see the following Remarks section.


### -param *pWbemServices [in]

Specifies a WMI services pointer to the RSoP namespace to which the policy data should be written. This parameter is <b>NULL</b> when RSoP logging is disabled, indicating that the extension should not log RSoP data.


### -param *pRsopStatus [out]

Pointer to an <b>HRESULT</b> return code that indicates whether RSoP logging was successful.


## -returns



If policy was applied successfully, return <b>ERROR_SUCCESS</b>. If there are no changes to the GPO list, and the extension is to be called again, return <b>ERROR_OVERRIDE_NOCHANGES</b>. Returning <b>ERROR_OVERRIDE_NOCHANGES</b> ensures that the extension is called again, even if the <b>NoGPOListChanges</b> registry value is set. (For more information about this registry value, see Remarks.)

Return <b>ERROR_SYNC_FOREGROUND_REFRESH_REQUIRED</b> if the function was called for an asynchronous foreground refresh of policy but policy could not be applied during the asynchronous refresh. Returning <b>ERROR_SYNC_FOREGROUND_REFRESH_REQUIRED</b> indicates that the function must be called again for a synchronous foreground refresh of policy.

Otherwise, return a 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>.




## -remarks



For more information, see 
<a href="https://msdn.microsoft.com/6124fa2f-f518-498f-ba07-210c2dbaca9a">Implementing a Group Policy Client-side Extension</a>.

The system calls this function in the context of the 
<a href="https://msdn.microsoft.com/692bceb6-f5bd-4b83-ab3b-ef8099dc84e1">LocalSystem account</a>, which has extensive privileges on the local computer. To use network resources, you must impersonate the user or computer by using the token provided in the <i>hToken</i> parameter.

To register this callback function, create a subkey under the following registry key:


<b>HKEY_LOCAL_MACHINE</b>\<b>SOFTWARE</b>\<b>Microsoft</b>\<b>Windows NT</b>\<b>CurrentVersion</b>\<b>Winlogon</b>\<b>GPExtensions</b>\<b>ClientExtensionGuid</b>



The subkey should be a <b>GUID</b>, so that it is unique. It should contain the following values.



You should update the status message only if you are applying policy synchronously. This allows you to provide feedback and diagnostics during a lengthy policy application. To use the status message callback function, you must verify that <i>pStatusCallback</i> is not <b>NULL</b>. Then load your message string resource. When you call the status function, you must indicate whether the string is verbose. If the string is verbose, the callback function will verify that the computer is in verbose mode and display the message. For more information, see 
<a href="https://msdn.microsoft.com/9eec6204-49b5-49fd-8db4-5c1777eb7c85">StatusMessageCallback</a>.

<div class="alert"><b>Warning</b>  Do not call the <i>pStatusCallback</i> function from a background thread or you may overwrite another thread's status message.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/7c45666e-d7c7-4989-ad19-b1b230757a88">Group Policy
    Functions</a>



<a href="https://msdn.microsoft.com/1285ab5a-ea68-4c16-bc34-8ab2f3cfad35">Group Policy
    Overview</a>



<a href="https://msdn.microsoft.com/f639c11c-ee65-45b6-ba0d-f39c825b3d80">ProcessGroupPolicy</a>



<a href="https://msdn.microsoft.com/0d899190-7345-4762-ab59-b89e2e87d10f">ProcessGroupPolicyCompletedEx</a>



<a href="https://msdn.microsoft.com/f1690fde-2390-4471-baba-70f4e805e245">RSOP_ExtensionStatus</a>



<a href="https://msdn.microsoft.com/e08cb006-d174-4506-87f0-580660bd4023">RefreshPolicy</a>



<a href="https://msdn.microsoft.com/905ab96b-a7f2-4bb4-a539-385f78284644">RefreshPolicyEx</a>



<a href="https://msdn.microsoft.com/9eec6204-49b5-49fd-8db4-5c1777eb7c85">StatusMessageCallback</a>
 

 

