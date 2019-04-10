---
UID: NF:mi.MI_Session_EnumerateClasses
title: MI_Session_EnumerateClasses function (mi.h)
author: windows-sdk-content
description: Enumerates the classes of a specified session.
old-location: wmi_v2\mi_session_enumerateclasses.htm
tech.root: wmi_v2
ms.assetid: eab78b29-2066-45ba-8e94-eb5dba322c23
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MI_Session_EnumerateClasses, MI_Session_EnumerateClasses function [Windows Management Infrastructure (MI)], mi/MI_Session_EnumerateClasses, wmi_v2.mi_session_enumerateclasses
ms.topic: function
req.header: mi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
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
 - HeaderDef
api_location:
 - Mi.h
api_name:
 - MI_Session_EnumerateClasses
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Management Framework 3.0 on Windows Server 2008 R2 with SP1, Windows 7 with SP1, and Windows Server 2008 with SP2
---

# MI_Session_EnumerateClasses function


## -description


Enumerates the classes of a specified session.


## -parameters




### -param session [in]

Session handle returned from <a href="https://msdn.microsoft.com/76010766-aa20-4632-940d-48d9769803da">MI_Application_NewSession</a>.


### -param flags

Runtime type information (RTTI) and polymorphism <a href="https://msdn.microsoft.com/24E82AC6-A2E3-4EC6-931F-26AC54D5CAA7">flags</a>.


### -param options [in, optional]

Optional <a href="https://msdn.microsoft.com/60445a53-c40c-4d0a-9650-21d0c7f3bbf6">MI_OperationOptions</a> value that specifies options such as timeouts and how to control the CIM semantics. Specify <b>Null</b> if no operation options are to be sent.


### -param namespaceName

An optional, null-terminated string that represents the namespace name to carry out the operation.  If none is specified, the server will pick a default.  The namespace cannot include a computer name.  It can only be in the form of a namespace name separated by a slash mark character (/). For example, the following would be a valid <b>namespaceName</b> value: <b>root/cimv2</b>.


### -param className

An optional, null-terminated string that represents the class name of the class to retrieve. If <b>Null</b>, the function retrieves all classes that are not derived from anything as well as all child classes (depending on the <b>options</b> parameter). If a class name is specified, this function retrieves all classes derived from the specified class as well as all child classes (depending on the <b>options</b> parameter).


### -param classNamesOnly

Boolean value where <b>MI_TRUE</b> means to retrieve only the class names and not properties. <b>MI_FALSE</b> means to retrieve all class properties.


### -param callbacks [in, optional]

Optional <a href="https://msdn.microsoft.com/f56954bf-c1aa-408b-bc45-0faf2a99b381">MI_OperationCallbacks</a> structure that defines the operational callbacks to receive the instance result and CIM semantics. Can be <b>NULL</b>. For asynchronous operation, the structure's <b>classResult</b> callback must be specified. If that value is not specified, then the client mus5t call the <a href="https://msdn.microsoft.com/f29f5a03-2b0b-4d36-97cb-f3b38f6037b3">MI_Operation_GetClass</a> function to retrieve the results.


### -param operation [out]

Returned operation handle that must be closed via <a href="https://msdn.microsoft.com/3e698e34-d537-4ea4-9345-cc4f493ff823">MI_Operation_Close</a> once complete.  Calling <a href="https://msdn.microsoft.com/11a9f9f6-9dfa-4f7c-9562-f4793c007f04">MI_Operation_Cancel</a> before it is complete will cause the operation to shutdown.  <b>MI_Operation_Close</b> and <b>MI_Operation_Cancel</b> can be called from any operation.


## -see-also




<a href="https://msdn.microsoft.com/76010766-aa20-4632-940d-48d9769803da">MI_Application_NewSession</a>



<a href="https://msdn.microsoft.com/f56954bf-c1aa-408b-bc45-0faf2a99b381">MI_OperationCallbacks</a>



<a href="https://msdn.microsoft.com/11a9f9f6-9dfa-4f7c-9562-f4793c007f04">MI_Operation_Cancel</a>



<a href="https://msdn.microsoft.com/3e698e34-d537-4ea4-9345-cc4f493ff823">MI_Operation_Close</a>



<a href="https://msdn.microsoft.com/f29f5a03-2b0b-4d36-97cb-f3b38f6037b3">MI_Operation_GetClass</a>
 

 

