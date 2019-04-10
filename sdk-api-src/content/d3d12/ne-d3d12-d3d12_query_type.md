---
UID: NE:d3d12.D3D12_QUERY_TYPE
title: D3D12_QUERY_TYPE (d3d12.h)
author: windows-sdk-content
description: Specifies the type of query.
old-location: direct3d12\d3d12_query_type.htm
tech.root: direct3d12
ms.assetid: F6FA9ACE-0089-4C7B-99D7-FD286CF4B18D
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: D3D12_QUERY_TYPE, D3D12_QUERY_TYPE enumeration, D3D12_QUERY_TYPE_BINARY_OCCLUSION, D3D12_QUERY_TYPE_OCCLUSION, D3D12_QUERY_TYPE_PIPELINE_STATISTICS, D3D12_QUERY_TYPE_SO_STATISTICS_STREAM0, D3D12_QUERY_TYPE_SO_STATISTICS_STREAM1, D3D12_QUERY_TYPE_SO_STATISTICS_STREAM2, D3D12_QUERY_TYPE_SO_STATISTICS_STREAM3, D3D12_QUERY_TYPE_TIMESTAMP, D3D12_QUERY_TYPE_VIDEO_DECODE_STATISTICS, d3d12/D3D12_QUERY_TYPE, d3d12/D3D12_QUERY_TYPE_BINARY_OCCLUSION, d3d12/D3D12_QUERY_TYPE_OCCLUSION, d3d12/D3D12_QUERY_TYPE_PIPELINE_STATISTICS, d3d12/D3D12_QUERY_TYPE_SO_STATISTICS_STREAM0, d3d12/D3D12_QUERY_TYPE_SO_STATISTICS_STREAM1, d3d12/D3D12_QUERY_TYPE_SO_STATISTICS_STREAM2, d3d12/D3D12_QUERY_TYPE_SO_STATISTICS_STREAM3, d3d12/D3D12_QUERY_TYPE_TIMESTAMP, d3d12/D3D12_QUERY_TYPE_VIDEO_DECODE_STATISTICS, direct3d12.d3d12_query_type
ms.topic: enum
req.header: d3d12.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - D3D12.h
api_name:
 - D3D12_QUERY_TYPE
product: Windows
targetos: Windows
req.typenames: D3D12_QUERY_TYPE
req.redist: 
---

# D3D12_QUERY_TYPE enumeration


## -description


Specifies the type of query.


## -enum-fields




### -field D3D12_QUERY_TYPE_OCCLUSION

Indicates the query is for depth/stencil occlusion counts.


### -field D3D12_QUERY_TYPE_BINARY_OCCLUSION

Indicates the query is for a binary depth/stencil occlusion statistics.

This new query type acts like D3D12_QUERY_TYPE_OCCLUSION except that it returns simply a binary 0/1 result:  0 indicates that no samples passed depth and stencil testing, 1 indicates that at least one sample passed depth and stencil testing.  This enables occlusion queries to not interfere with any GPU performance optimization associated with depth/stencil testing.


### -field D3D12_QUERY_TYPE_TIMESTAMP

Indicates the query is for high definition GPU and CPU timestamps.


### -field D3D12_QUERY_TYPE_PIPELINE_STATISTICS

Indicates the query type is for graphics pipeline statistics, refer to <a href="https://msdn.microsoft.com/0A84A3C8-0F6F-420E-88C9-26EC03F03179">D3D12_QUERY_DATA_PIPELINE_STATISTICS</a>.


### -field D3D12_QUERY_TYPE_SO_STATISTICS_STREAM0

Stream 0 output statistics. In Direct3D 12 there is no single stream output (SO) overflow query for all the output streams. Apps need to issue multiple single-stream queries, and then correlate the results. Stream output is the ability of the GPU to write vertices to a buffer. The stream output counters monitor progress.


### -field D3D12_QUERY_TYPE_SO_STATISTICS_STREAM1

Stream 1 output statistics.


### -field D3D12_QUERY_TYPE_SO_STATISTICS_STREAM2

Stream 2 output statistics.


### -field D3D12_QUERY_TYPE_SO_STATISTICS_STREAM3

Stream 3 output statistics.


### -field D3D12_QUERY_TYPE_VIDEO_DECODE_STATISTICS

Video decode statistics. Refer to <a href="direct3d12.d3d12_query_data_video_decode_statistics">D3D12_QUERY_DATA_VIDEO_DECODE_STATISTICS</a>.

Use this query type to determine if a video was successfully decoded. If decoding fails due to insufficient BitRate or FrameRate parameters set during creation of the decode heap, then the status field of the query is set to D3D12_VIDEO_DECODE_STATUS_RATE_EXCEEDED and the query also contains new BitRate and FrameRate values that would succeed.

This query type can only be performed on video decode command lists (<a href="https://msdn.microsoft.com/28BC70FF-6818-4B8D-9DE4-8316AB2FB288">D3D12_COMMAND_LIST_TYPE_VIDEO_DECODE</a>). This query type does not use <a href="direct3d12.id3d12videodecodecommandlist_beginquery">ID3D12VideoDecodeCommandList::BeginQuery</a>, only <a href="direct3d12.id3d12videodecodecommandlist_endquery">ID3D12VideoDecoeCommandList::EndQuery</a>. Statistics are recorded only for the most recent <a href="direct3d12.id3d12videodecodecommandlist_decodeframe">ID3D12VideoDecoeCommandList::DecodeFrame</a> call in the same command list.


## -remarks



This enum is used by <a href="https://msdn.microsoft.com/38011ED8-C867-4ECE-880F-3963A17790F7">BeginQuery</a>, <a href="https://msdn.microsoft.com/591B277C-44C7-4C21-86B1-239F6A71308D">EndQuery</a> and <a href="https://msdn.microsoft.com/E3154DB7-DDA9-4480-A918-19C3A62944F2">ResolveQueryData.</a>





## -see-also




<a href="https://msdn.microsoft.com/76E76C85-128E-4F0E-9711-C72C4CF6C835">Core Enumerations</a>
 

 

