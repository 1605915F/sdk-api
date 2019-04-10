---
UID: NF:wmdmlog.IWMDMLogger.LogString
title: IWMDMLogger::LogString (wmdmlog.h)
author: windows-sdk-content
description: The LogString method logs a string to the current log file. A carriage return and line feed are added to each log entry.
old-location: wmdm\iwmdmlogger_logstring.htm
tech.root: WMDM
ms.assetid: 6a084ef6-20dc-4363-b9b8-c4e9bcb1dd71
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMDMLogger interface [windows Media Device Manager],LogString method, IWMDMLogger.LogString, IWMDMLogger::LogString, IWMDMLoggerLogString, LogString, LogString method [windows Media Device Manager], LogString method [windows Media Device Manager],IWMDMLogger interface, wmdm.iwmdmlogger_logstring, wmdmlog/IWMDMLogger::LogString
ms.topic: method
req.header: wmdmlog.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mssachlp.lib
 - mssachlp.dll
api_name:
 - IWMDMLogger.LogString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMLogger::LogString


## -description



The <b>LogString</b> method logs a string to the current log file. A carriage return and line feed are added to each log entry.




## -parameters




### -param dwFlags [in]

Flags that control the way a string is logged. This parameter is a combination of one or more of the following values.

<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>WMDM_LOG_SEV_INFO</td>
<td>Tag the log entry as informational.</td>
</tr>
<tr>
<td>WMDM_LOG_SEV_WARN</td>
<td>Tag the log entry as a warning.</td>
</tr>
<tr>
<td>WMDM_LOG_SEV_ERROR</td>
<td>Tag the log entry as an error.</td>
</tr>
<tr>
<td>WMDM_LOG_NOTIMESTAMP</td>
<td>Do not include a time stamp on the log entry. Time stamps are in ISO format minus the time-zone information.</td>
</tr>
</table>
 


### -param pszSrcName [in]

Pointer to a string containing the name of the module that is making the log entry. This parameter can be <b>NULL</b>.


### -param pszLog [in]

Pointer to a string to be copied to the log. This parameter can be <b>NULL</b>.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/50fc1d71-b650-4ba5-a6e1-631c0b9fe8ad">Enabling Logging</a>



<a href="https://msdn.microsoft.com/bededb91-f343-455b-a3ef-548e6f961933">IWMDMLogger Interface</a>
 

 

