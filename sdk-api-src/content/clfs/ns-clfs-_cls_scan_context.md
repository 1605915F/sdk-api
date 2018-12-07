---
UID: NS:clfs._CLS_SCAN_CONTEXT
title: "_CLS_SCAN_CONTEXT"
author: windows-sdk-content
description: Contains information about the containers that are being scanned by ScanLogContainers, the kind of scan that is being performed, and a cursor to track which containers have been scanned.
old-location: fs\clfs_scan_context.htm
tech.root: Clfs
ms.assetid: 716fa005-c801-4a5d-99f1-0babe64dc4a8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCLFS_SCAN_CONTEXT, *PCLS_SCAN_CONTEXT, CLFS_SCAN_BACKWARD, CLFS_SCAN_CLOSE, CLFS_SCAN_CONTEXT, CLFS_SCAN_CONTEXT structure [Files], CLFS_SCAN_FORWARD, CLFS_SCAN_INIT, CLS_SCAN_CONTEXT, PCLFS_SCAN_CONTEXT, PCLFS_SCAN_CONTEXT structure pointer [Files], PPCLS_SCAN_CONTEXT, _CLS_SCAN_CONTEXT, clfs/PCLFS_SCAN_CONTEXT, clfs/_CLFS_SCAN_CONTEXT, fs.clfs_scan_context"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: clfs.h
req.include-header: Clfsw32.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
 - Clfs.h
api_name:
 - CLFS_SCAN_CONTEXT
product: Windows
targetos: Windows
req.typenames: CLS_SCAN_CONTEXT, *PCLS_SCAN_CONTEXT, PPCLS_SCAN_CONTEXT
req.redist: 
---

# _CLS_SCAN_CONTEXT structure


## -description


Contains information about the containers that are being scanned by <a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a>, the kind of scan that is being performed, and a  cursor to track which containers have been scanned.


## -struct-fields




### -field cidNode

The ID of the current node. For more information, see <a href="https://msdn.microsoft.com/en-us/library/Bb891960(v=VS.85).aspx">CLFS_NODE_ID</a>.


### -field plfoLog

 


### -field cIndex

The index of the current container.


### -field cContainers

The number of system-allocated <a href="https://msdn.microsoft.com/en-us/library/Bb540336(v=VS.85).aspx">CLFS_CONTAINER_INFORMATION</a> structures in an array that is pointed to by <b>pinfoContainer</b>. 

That is, this member is the number of containers to scan with each scan call.   The caller knows the scan is complete when the number of containers returned is less than this value.


### -field cContainersReturned

The number of containers that are returned after a call to <a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a>.


### -field eScanMode

The mode in which containers are scanned.  

Containers can be scanned in one of the following modes.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="CLFS_SCAN_INIT"></a><a id="clfs_scan_init"></a><dl>
<dt><b>CLFS_SCAN_INIT</b></dt>
</dl>
</td>
<td width="60%">
Initializes the scan context, but does not allocate associated storage.  

The initialization is destructive, because all  data that is stored in the current scan context is lost.

</td>
</tr>
<tr>
<td width="40%"><a id="CLFS_SCAN_CLOSE"></a><a id="clfs_scan_close"></a><dl>
<dt><b>CLFS_SCAN_CLOSE</b></dt>
</dl>
</td>
<td width="60%">
Uninitializes the scan context and deallocates  system storage that is associated with a scan context.

</td>
</tr>
<tr>
<td width="40%"><a id="CLFS_SCAN_FORWARD"></a><a id="clfs_scan_forward"></a><dl>
<dt><b>CLFS_SCAN_FORWARD</b></dt>
</dl>
</td>
<td width="60%">
Causes the next call to <a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a> to proceed  in a forward direction. 

Cannot be used if <b>CLFS_SCAN_BACKWARD</b> is specified.

</td>
</tr>
<tr>
<td width="40%"><a id="CLFS_SCAN_BACKWARD"></a><a id="clfs_scan_backward"></a><dl>
<dt><b>CLFS_SCAN_BACKWARD</b></dt>
</dl>
</td>
<td width="60%">
Causes the next call to <a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a> to proceed  in a backward direction. 

Cannot be used if <b>CLFS_SCAN_FORWARD</b> is specified.

</td>
</tr>
</table>
 


### -field pinfoContainer

A pointer to
					a client-allocated array of <a href="https://msdn.microsoft.com/en-us/library/Bb540336(v=VS.85).aspx">CLFS_CONTAINER_INFORMATION</a> structures to be filled by <a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a> after each successful call.


#### - hLog

A handle to the log being scanned that is obtained from <a href="https://msdn.microsoft.com/en-us/library/Bb540366(v=VS.85).aspx">CreateLogFile</a> with permissions  to scan the log containers.  


## -remarks



This structure is allocated by the client, initialized using <a href="https://msdn.microsoft.com/en-us/library/Bb540365(v=VS.85).aspx">CreateLogContainerScanContext</a>, and then passed to <a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a> in repeated calls.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb540336(v=VS.85).aspx">CLFS_CONTAINER_INFORMATION</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb891960(v=VS.85).aspx">CLFS_NODE_ID</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb525003(v=VS.85).aspx">ScanLogContainers</a>
 

 

