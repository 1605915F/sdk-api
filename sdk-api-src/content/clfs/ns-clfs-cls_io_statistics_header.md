---
UID: NS:clfs._CLS_IO_STATISTICS_HEADER
title: CLS_IO_STATISTICS_HEADER (clfs.h)
author: windows-sdk-content
description: Header for information retrieved by the GetLogIoStatistics function, which defines the I/O performance counters of a log.
old-location: fs\clfs_io_statistics_header.htm
tech.root: Clfs
ms.assetid: ebf3f962-5c15-4caf-910a-13bf02137046
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PCLFS_IO_STATISTICS_HEADER, *PCLS_IO_STATISTICS_HEADER, CLFS_IO_STATISTICS_HEADER, CLFS_IO_STATISTICS_HEADER structure [Files], CLS_IO_STATISTICS_HEADER, PCLFS_IO_STATISTICS_HEADER, PCLFS_IO_STATISTICS_HEADER structure pointer [Files], PPCLFS_IO_STATISTICS_HEADER, PPCLFS_IO_STATISTICS_HEADER structure pointer [Files], PPCLS_IO_STATISTICS_HEADER, clfs/PCLFS_IO_STATISTICS_HEADER, clfs/PPCLFS_IO_STATISTICS_HEADER, clfs/_CLFS_IO_STATISTICS_HEADER, fs.clfs_io_statistics_header"
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
 - CLFS_IO_STATISTICS_HEADER
product: Windows
targetos: Windows
req.typenames: CLS_IO_STATISTICS_HEADER, *PCLS_IO_STATISTICS_HEADER, PPCLS_IO_STATISTICS_HEADER
req.redist: 
---

# CLS_IO_STATISTICS_HEADER structure


## -description


Header for information retrieved by the <a href="https://msdn.microsoft.com/1d4a5486-8a9e-480a-952c-12fc7386af3e">GetLogIoStatistics</a> function, which defines the I/O performance counters of a log.


## -struct-fields




### -field ubMajorVersion

The major version of the statistics buffer.


### -field ubMinorVersion

The minor version of the statistics buffer.


### -field eStatsClass

The class of I/O statistics  that is exported. Currently, flush statistics are the only statistics information exported.  These statistics  include the frequency of data and metadata flushes on a dedicated log and the amount of data and metadata flushed. Because  flush statistics are  the  sole statistics class, this member is currently unused but will be used in the future.


### -field cbLength

The length of the statistics buffer, including the header.


### -field coffData

The offset of statistics counters from the beginning of the packet where the statistics data begins.  This field allows transparent modifications to the header and length without affecting  how the statistics data is accessed. 


## -remarks



This header is followed by the I/O statistics counters.




## -see-also




<a href="https://msdn.microsoft.com/8ba1f5e4-9af3-4c8a-8b57-b6075d0560d6">CLFS_IOSTATS_CLASS</a>



<a href="https://msdn.microsoft.com/99544331-0a7c-4efd-93a7-e94011375394">CLFS_IO_STATISTICS</a>



<a href="https://msdn.microsoft.com/1d4a5486-8a9e-480a-952c-12fc7386af3e">GetLogIoStatistics</a>
 

 

