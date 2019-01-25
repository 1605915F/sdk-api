---
UID: NF:tapi.lineGetCountry
title: lineGetCountry function
author: windows-sdk-content
description: The lineGetCountry function fetches the stored dialing rules and other information related to a specified country/region, the first country/region in the country/region list, or all countries/regions.
old-location: tapi2\linegetcountry.htm
tech.root: Tapi
ms.assetid: 4de271b3-d93b-4fc9-b853-e26ef1ae75ae
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_tapi2_linegetcountry, lineGetCountry, lineGetCountry function [TAPI 2.2], lineGetCountryA, lineGetCountryW, tapi/lineGetCountry, tapi/lineGetCountryA, tapi/lineGetCountryW, tapi2.linegetcountry"
ms.topic: function
req.header: tapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: lineGetCountryW (Unicode) and lineGetCountryA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Tapi32.lib
req.dll: Tapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Tapi32.dll
api_name:
 - lineGetCountry
 - lineGetCountryA
 - lineGetCountryW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# lineGetCountry function


## -description


The 
<b>lineGetCountry</b> function fetches the stored dialing rules and other information related to a specified country/region, the first country/region in the country/region list, or all countries/regions.


## -parameters




### -param dwCountryID

Country/region identifier (not the country code) of the country/region for which information is to be obtained. If the value 1 is specified, information on the first country/region in the country/region list is obtained. If the value 0 is specified, information on all countries/regions is obtained (which can require a great deal of memory — 20 KB or more).


### -param dwAPIVersion

Highest version of TAPI supported by the application (not necessarily the value negotiated by 
<a href="https://msdn.microsoft.com/71eb55de-281b-42a9-8d9b-7ded62cb006a">lineNegotiateAPIVersion</a> on some particular line device).


### -param lpLineCountryList

Pointer to a location to which a <a href="https://msdn.microsoft.com/f6634d40-0c17-4eb1-a0ca-9590e9e649e2">LINECOUNTRYLIST</a> structure is loaded. Prior to calling 
<b>lineGetCountry</b>, the application must set the <b>dwTotalSize</b> member of this structure to indicate the amount of memory available to TAPI for returning information. 




<div class="alert"><b>Note</b>  If the size parameters in the structure are not correct, there is a possibility that data could get overwritten. For more information on setting structure sizes, see the 
<a href="https://msdn.microsoft.com/61313fe3-74a1-4195-b5af-37463dad02c1">memory allocation</a> topic.</div>
<div> </div>

## -returns



Returns zero if the request succeeds or a negative error number if an error occurs. Possible return values are:

LINEERR_INCOMPATIBLEAPIVERSION, LINEERR_NOMEM, LINEERR_INIFILECORRUPT, LINEERR_OPERATIONFAILED, LINEERR_INVALCOUNTRYCODE, LINEERR_STRUCTURETOOSMALL, LINEERR_INVALPOINTER.




## -see-also




<a href="https://msdn.microsoft.com/09d10789-bc36-47c7-b77d-8698ae75541a">Basic Telephony Services Reference</a>



<a href="https://msdn.microsoft.com/f6634d40-0c17-4eb1-a0ca-9590e9e649e2">LINECOUNTRYLIST</a>



<a href="https://msdn.microsoft.com/d703b414-1389-416c-8e94-c1931979f0c9">TAPI 2.2 Reference Overview</a>



<a href="https://msdn.microsoft.com/71eb55de-281b-42a9-8d9b-7ded62cb006a">lineNegotiateAPIVersion</a>
 

 

