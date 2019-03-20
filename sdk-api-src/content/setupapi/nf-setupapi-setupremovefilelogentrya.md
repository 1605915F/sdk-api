---
UID: NF:setupapi.SetupRemoveFileLogEntryA
title: SetupRemoveFileLogEntryA function (setupapi.h)
author: windows-sdk-content
description: The SetupRemoveFileLogEntry function removes an entry or section from a file log.
old-location: setup\setupremovefilelogentry.htm
tech.root: SetupApi
ms.assetid: a26d2c24-7092-40b0-9ae9-e7edf68aeb3d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetupRemoveFileLogEntry, SetupRemoveFileLogEntry function [Setup API], SetupRemoveFileLogEntryA, SetupRemoveFileLogEntryW, _setupapi_setupremovefilelogentry, setup.setupremovefilelogentry, setupapi/SetupRemoveFileLogEntry, setupapi/SetupRemoveFileLogEntryA, setupapi/SetupRemoveFileLogEntryW
ms.topic: function
req.header: setupapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SetupRemoveFileLogEntryW (Unicode) and SetupRemoveFileLogEntryA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Setupapi.dll
api_name:
 - SetupRemoveFileLogEntry
 - SetupRemoveFileLogEntryA
 - SetupRemoveFileLogEntryW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetupRemoveFileLogEntryA function


## -description


<p class="CCE_Message">[This function is available for use in the operating systems indicated in the Requirements section. It may be altered or unavailable in subsequent versions.   SetupAPI should no longer be used for installing applications. Instead, use the Windows Installer for developing application installers. SetupAPI continues to be used for installing device drivers.]

The 
<b>SetupRemoveFileLogEntry</b> function removes an entry or section from a file log.


## -parameters




### -param FileLogHandle [in]

Handle to the file log as returned by 
<a href="https://msdn.microsoft.com/fac7abac-76a9-456a-843a-e1048df268b7">SetupInitializeFileLog</a>. The caller must not have passed SPFILELOG_QUERYONLY when the log file was initialized.


### -param LogSectionName [in]

Pointer to a <b>null</b>-terminated string that specifies the name for a logical grouping of names within the log file. Required for non-system logs. Otherwise, <i>LogSectionName</i> may be <b>NULL</b>.


### -param TargetFilename [in]

Pointer to a <b>null</b>-terminated string that specifies the name of the file as it exists on the target. This name should be in whatever format is meaningful to the caller. If <b>NULL</b>, the section specified by <i>LogSectionName</i> is removed. The main section cannot be removed.


## -returns



If the function succeeds, the return value is a nonzero value.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -see-also




<a href="https://msdn.microsoft.com/0a9518b7-f231-48f2-ba50-5b802f8ccaed">Functions</a>



<a href="https://msdn.microsoft.com/58201596-cb8c-480a-abef-896c1f9ef098">Overview</a>



<a href="https://msdn.microsoft.com/bc738212-ff81-4b52-b2ef-50aabf6658ab">SetupLogFile</a>
 

 

