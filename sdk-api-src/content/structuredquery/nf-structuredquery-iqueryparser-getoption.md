---
UID: NF:structuredquery.IQueryParser.GetOption
title: IQueryParser::GetOption (structuredquery.h)
author: windows-sdk-content
description: Retrieves a specified simple option value for this query parser.
old-location: search\_search_IQueryParser_GetOption.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\querying\iqueryparser\getoption.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetOption, GetOption method [search], GetOption method [search],IQueryParser interface, IQueryParser interface [search],GetOption method, IQueryParser.GetOption, IQueryParser::GetOption, _search_IQueryParser_GetOption, search._search_IQueryParser_GetOption, structuredquery/IQueryParser::GetOption
ms.topic: method
req.header: structuredquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Structuredquery.idl
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
 - COM
api_location:
 - Structuredquery.h
api_name:
 - IQueryParser.GetOption
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# IQueryParser::GetOption


## -description


Retrieves a specified simple option value for this query parser.


## -parameters




### -param option [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa965708(v=VS.85).aspx">STRUCTURED_QUERY_SINGLE_OPTION</a></b>

The <a href="https://msdn.microsoft.com/en-us/library/Aa965708(v=VS.85).aspx">STRUCTURED_QUERY_SINGLE_OPTION</a> enumerated type that specifies the option to be retrieved.
        


### -param pOptionValue [out, retval]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa380072(v=VS.85).aspx">PROPVARIANT</a>*</b>

Receives a pointer to the specified option value. For more information, see <a href="https://msdn.microsoft.com/en-us/library/Aa965708(v=VS.85).aspx">STRUCTURED_QUERY_SINGLE_OPTION</a>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



