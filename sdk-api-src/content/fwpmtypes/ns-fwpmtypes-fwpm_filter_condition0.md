---
UID: NS:fwpmtypes.FWPM_FILTER_CONDITION0_
title: FWPM_FILTER_CONDITION0 (fwpmtypes.h)
author: windows-sdk-content
description: Expresses a filter condition that must be true for the action to be taken.
old-location: fwp\fwpm_filter_condition0_struct.htm
tech.root: fwp
ms.assetid: 4dfed9d7-e51b-425c-9f27-014229c140be
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FWPM_FILTER_CONDITION0, FWPM_FILTER_CONDITION0 structure [Filtering], fwp.fwpm_filter_condition0_struct, fwpmtypes/FWPM_FILTER_CONDITION0
ms.topic: struct
req.header: fwpmtypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Fwpmtypes.idl
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
 - Fwpmtypes.h
api_name:
 - FWPM_FILTER_CONDITION0
product: Windows
targetos: Windows
req.typenames: FWPM_FILTER_CONDITION0
req.redist: 
ms.custom: 19H1
---

# FWPM_FILTER_CONDITION0 structure


## -description


The <b>FWPM_FILTER_CONDITION0</b> structure expresses a filter condition that must be true for the action to be taken.


## -struct-fields




### -field fieldKey

GUID of the field to be tested.


### -field matchType

A <a href="https://msdn.microsoft.com/a49efb25-990c-459d-90bc-758337c351d5">FWP_MATCH_TYPE</a> value that specifies the type of match to be performed.


### -field conditionValue

A <a href="https://msdn.microsoft.com/edc34005-dbc1-45a4-b6c7-fbb8b13fa388">FWP_CONDITION_VALUE0</a> structure that contains the value to match the field against.


## -remarks



Field GUIDs are
   only unique within a layer, so both the field GUID and the layer GUID are required to uniquely identify a
   field.

The data type of 
<b>conditionValue</b> must be compatible with the <b>matchType</b> value. See <a href="https://msdn.microsoft.com/a49efb25-990c-459d-90bc-758337c351d5">FWP_MATCH_TYPE</a> for detailed  compatibility rules.

<b>FWPM_FILTER_CONDITION0</b> is a specific implementation of FWPM_FILTER_CONDITION. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a>  for more information.


#### Examples

The following C++ example shows how to initialize and add conditions to a filter.


```cpp
#include <windows.h>
#include <fwpmu.h>
#include <stdio.h>

#pragma comment(lib, "Fwpuclnt.lib")

// Some application to use for filter testing.
#define FILE0_PATH L"C:\\Program Files\\AppDirectory\\SomeApplication.exe"

void main()
{
    FWP_BYTE_BLOB *fwpApplicationByteBlob;
    FWPM_FILTER0 fwpFilter;
    FWPM_FILTER_CONDITION0 fwpConditions[4];
    int conCount = 0;
    DWORD result = ERROR_SUCCESS; 

    fwpApplicationByteBlob = (FWP_BYTE_BLOB*) malloc(sizeof(FWP_BYTE_BLOB));
    
    printf("Retrieving application identifier for filter testing.\n"); 
    result = FwpmGetAppIdFromFileName0(FILE0_PATH, &fwpApplicationByteBlob);
    if (result != ERROR_SUCCESS)
    {
        printf("FwpmGetAppIdFromFileName failed (%d).\n", result);
        return;
    }

      // Application identifier filter condition.
      fwpConditions[conCount].fieldKey = FWPM_CONDITION_ALE_APP_ID;
      fwpConditions[conCount].matchType = FWP_MATCH_EQUAL;
      fwpConditions[conCount].conditionValue.type = FWP_BYTE_BLOB_TYPE;
      fwpConditions[conCount].conditionValue.byteBlob = fwpApplicationByteBlob;
            
      ++conCount;

      // TCP protocol filter condition
      fwpConditions[conCount].fieldKey = FWPM_CONDITION_IP_PROTOCOL;
      fwpConditions[conCount].matchType = FWP_MATCH_EQUAL;
      fwpConditions[conCount].conditionValue.type = FWP_UINT8;
      fwpConditions[conCount].conditionValue.uint8 = IPPROTO_TCP;

      ++conCount;

      // Add conditions and condition count to a filter.
      memset(&fwpFilter, 0, sizeof(FWPM_FILTER0));

      fwpFilter.numFilterConditions = conCount;
      if (conCount > 0)
        fwpFilter.filterCondition = fwpConditions;

      // Finish initializing filter...

    return;
}

```





## -see-also




<a href="https://msdn.microsoft.com/edc34005-dbc1-45a4-b6c7-fbb8b13fa388">FWP_CONDITION_VALUE0</a>



<a href="https://msdn.microsoft.com/a49efb25-990c-459d-90bc-758337c351d5">FWP_MATCH_TYPE</a>



<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 

