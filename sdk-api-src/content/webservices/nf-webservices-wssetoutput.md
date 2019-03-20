---
UID: NF:webservices.WsSetOutput
title: WsSetOutput function (webservices.h)
author: windows-sdk-content
description: Sets the encoding and output callbacks for the writer. The callbacks are used to provides buffers to the writer and to perform asynchronous i/o.
old-location: wsw\wssetoutput.htm
tech.root: wsw
ms.assetid: f0b47817-0ad1-408c-a6da-9a7b0fb2e34b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WsSetOutput, WsSetOutput function [Web Services for Windows], webservices/WsSetOutput, wsw.wssetoutput
ms.topic: function
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WebServices.lib
req.dll: WebServices.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - WebServices.dll
api_name:
 - WsSetOutput
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WsSetOutput function


## -description


Sets the encoding and output callbacks for the writer.  The callbacks are used to 
        provides buffers to the writer and to perform asynchronous i/o.
      


## -parameters




### -param writer [in]

The writer for which the output will be set.
        


### -param encoding [in, optional]

The encoding describes the format of the input bytes.  This should be one of <a href="https://msdn.microsoft.com/en-us/library/Dd323586(v=VS.85).aspx">WS_XML_WRITER_TEXT_ENCODING</a>,
          <a href="https://msdn.microsoft.com/en-us/library/Dd323574(v=VS.85).aspx">WS_XML_WRITER_BINARY_ENCODING</a> or <a href="https://msdn.microsoft.com/en-us/library/Dd323578(v=VS.85).aspx">WS_XML_WRITER_MTOM_ENCODING</a>.
        


### -param output [in, optional]

Specifies where the writer should place its data.
        


### -param properties

An array of optional properties of the writer.  See <a href="https://msdn.microsoft.com/2979d038-f0a8-407d-bf8e-dca4027f6410">WS_XML_WRITER_PROPERTY</a>.
        


### -param propertyCount [in]

The number of properties.


### -param error [in, optional]

Specifies where additional error information should be stored if the function fails.
        


## -returns



This function can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One or more arguments are invalid.

</td>
</tr>
</table>
 




## -remarks



When <b>WsSetOutput</b> is used on the writer, the writer will function in a forward only manner and
        the functions <a href="https://msdn.microsoft.com/0c0fbd78-ed4f-40da-a63d-a2f38136ecb3">WsGetWriterPosition</a>, <a href="https://msdn.microsoft.com/1d23bda1-d1da-44d4-9a9d-258bba200b29">WsSetWriterPosition</a> and <a href="https://msdn.microsoft.com/f8eace53-9fa5-466a-8894-3c8b8fe049e3">WsMoveWriter</a> cannot be used.
      

If <a href="https://msdn.microsoft.com/5ca43d39-e714-4070-b343-6c8ab9484817">encoding</a> is <b>NULL</b>, then <a href="https://msdn.microsoft.com/367e6f98-9351-4a08-b8ce-036e7f2788e4">WS_XML_WRITER_OUTPUT</a> is ignored and the writer is set up so that any attempt to write to it will fail.
      

If <a href="https://msdn.microsoft.com/5ca43d39-e714-4070-b343-6c8ab9484817">encoding</a> is not <b>NULL</b>, then <a href="https://msdn.microsoft.com/367e6f98-9351-4a08-b8ce-036e7f2788e4">WS_XML_WRITER_OUTPUT</a> must be non-<b>NULL</b> as well.
      

If <a href="https://msdn.microsoft.com/367e6f98-9351-4a08-b8ce-036e7f2788e4">WS_XML_WRITER_OUTPUT</a> is <a href="https://msdn.microsoft.com/en-us/library/Dd323575(v=VS.85).aspx">WS_XML_WRITER_BUFFER_OUTPUT</a> then the writer will buffer the generated
        bytes of the document.  Use <a href="https://msdn.microsoft.com/1167662f-0383-44bb-a7e1-1ec12539903e">WsGetWriterProperty</a> with <a href="https://msdn.microsoft.com/c919eb01-bd15-4583-afcf-e46ac2fc9c8c">WS_XML_WRITER_PROPERTY_BUFFERS</a> or
        <b>WS_XML_WRITER_PROPERTY_BYTES</b> to obtain these bytes.  In this mode <a href="https://msdn.microsoft.com/ba631942-d5a0-4d93-9899-c3f0ebd4aae5">WsFlushWriter</a> has no effect.
      

If <a href="https://msdn.microsoft.com/367e6f98-9351-4a08-b8ce-036e7f2788e4">WS_XML_WRITER_OUTPUT</a> is <a href="https://msdn.microsoft.com/en-us/library/Dd323585(v=VS.85).aspx">WS_XML_WRITER_STREAM_OUTPUT</a> then the writer will pass the generated
        bytes of the document to the specified <a href="https://msdn.microsoft.com/8d106ac2-226d-4e0c-8f14-8d3e17f15548">WS_WRITE_CALLBACK</a> during calls to <a href="https://msdn.microsoft.com/ba631942-d5a0-4d93-9899-c3f0ebd4aae5">WsFlushWriter</a>.
      

The writer will be initialized to use the properties specified in <a href="https://msdn.microsoft.com/5b4bb009-764e-4892-903a-5939f5570016">WsCreateWriter</a>.  Any properties
        specified to <b>WsSetOutput</b> will override those properties.
      

See <a href="https://msdn.microsoft.com/5b4bb009-764e-4892-903a-5939f5570016">WsCreateWriter</a> for the default values of the properties of the writer.
      



