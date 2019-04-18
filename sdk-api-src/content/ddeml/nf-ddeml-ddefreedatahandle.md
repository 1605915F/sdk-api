---
UID: NF:ddeml.DdeFreeDataHandle
title: DdeFreeDataHandle function (ddeml.h)
author: windows-sdk-content
description: Frees a Dynamic Data Exchange (DDE) object and deletes the data handle associated with the object.
old-location: dataxchg\ddefreedatahandle.htm
tech.root: dataxchg
ms.assetid: VS|winui|~\winui\windowsuserinterface\dataexchange\dynamicdataexchangemanagementlibrary\dynamicdataexchangemanagementreference\dynamicdataexchangemanagementfunctions\ddefreedatahandle.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DdeFreeDataHandle, DdeFreeDataHandle function [Data Exchange], _win32_DdeFreeDataHandle, _win32_ddefreedatahandle_cpp, dataxchg.ddefreedatahandle, ddeml/DdeFreeDataHandle, winui._win32_ddefreedatahandle
ms.topic: function
req.header: ddeml.h
req.include-header: Windows.h
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
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
api_name:
 - DdeFreeDataHandle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DdeFreeDataHandle function


## -description


Frees a Dynamic Data Exchange (DDE) object and deletes the data handle associated with the object. 


## -parameters




### -param hData [in]

Type: <b>HDDEDATA</b>

A handle to the DDE object to be freed. This handle must have been created by a previous call to the <a href="https://msdn.microsoft.com/en-us/library/ms648747(v=VS.85).aspx">DdeCreateDataHandle</a> function or returned by the <a href="https://msdn.microsoft.com/en-us/library/ms648743(v=VS.85).aspx">DdeClientTransaction</a> function. 


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. 

The <a href="https://msdn.microsoft.com/en-us/library/ms648755(v=VS.85).aspx">DdeGetLastError</a> function can be used to get the error code, which can be one of the following values: 




## -remarks



An application must call <b>DdeFreeDataHandle</b> under the following circumstances: 

<ul>
<li>To free a DDE object that the application allocated by calling the <a href="https://msdn.microsoft.com/en-us/library/ms648747(v=VS.85).aspx">DdeCreateDataHandle</a> function if the object's data handle was never passed by the application to another Dynamic Data Exchange Management Library (DDEML) function </li>
<li>To free a DDE object that the application allocated by specifying the <b>HDATA_APPOWNED</b> flag in a call to <a href="https://msdn.microsoft.com/en-us/library/ms648747(v=VS.85).aspx">DdeCreateDataHandle</a>
</li>
<li>To free a DDE object whose handle the application received from the <a href="https://msdn.microsoft.com/en-us/library/ms648743(v=VS.85).aspx">DdeClientTransaction</a> function </li>
</ul>
The system automatically frees an unowned object when its handle is returned by a DDE callback function or is used as a parameter in a DDEML function. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms648740(v=VS.85).aspx">DdeAccessData</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648743(v=VS.85).aspx">DdeClientTransaction</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648747(v=VS.85).aspx">DdeCreateDataHandle</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648712(v=VS.85).aspx">Dynamic Data Exchange Management Library</a>



<b>Reference</b>
 

 

