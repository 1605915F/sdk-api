---
UID: NF:mmdeviceapi.IMMNotificationClient.OnPropertyValueChanged
title: IMMNotificationClient::OnPropertyValueChanged
author: windows-sdk-content
description: The OnPropertyValueChanged method indicates that the value of a property belonging to an audio endpoint device has changed.
old-location: coreaudio\immnotificationclient_onpropertyvaluechanged.htm
tech.root: CoreAudio
ms.assetid: 194aa7d1-4885-49c4-b9c3-2c47468c139f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMMNotificationClient interface [Core Audio],OnPropertyValueChanged method, IMMNotificationClient.OnPropertyValueChanged, IMMNotificationClient::OnPropertyValueChanged, IMMNotificationClientOnPropertyValueChanged, OnPropertyValueChanged, OnPropertyValueChanged method [Core Audio], OnPropertyValueChanged method [Core Audio],IMMNotificationClient interface, coreaudio.immnotificationclient_onpropertyvaluechanged, mmdeviceapi/IMMNotificationClient::OnPropertyValueChanged
ms.topic: method
req.header: mmdeviceapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - COM
api_location:
 - Mmdeviceapi.h
api_name:
 - IMMNotificationClient.OnPropertyValueChanged
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMMNotificationClient::OnPropertyValueChanged


## -description



The <b>OnPropertyValueChanged</b> method indicates that the value of a property belonging to an audio endpoint device has changed.




## -parameters




### -param pwstrDeviceId [in]

Pointer to the <a href="https://msdn.microsoft.com/3c955e2d-daaa-4b77-8ca5-890383bb2d39">endpoint ID string</a> that identifies the audio endpoint device. This parameter points to a null-terminated, wide-character string that contains the endpoint ID. The string remains valid for the duration of the call.


### -param key [in]

A <a href="https://msdn.microsoft.com/3f5f31af-f040-443b-9045-9761055381ea">PROPERTYKEY</a> structure that specifies the property. The structure contains the property-set GUID and an index identifying a property within the set. The structure is passed by value. It remains valid for the duration of the call. For more information about <b>PROPERTYKEY</b>, see the Windows SDK documentation.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -remarks



A call to the <a href="https://msdn.microsoft.com/f5ede696-0cd4-41e2-9576-822e3f9909e7">IPropertyStore::SetValue</a> method that successfully changes the value of a property of an audio endpoint device generates a call to <b>OnPropertyValueChanged</b>. For more information about <b>IPropertyStore::SetValue</b>, see the Windows SDK documentation.

A client can use the <i>key</i> parameter to retrieve the new property value. For a code example that uses a property key to retrieve a property value from the property store of an endpoint device, see <a href="https://msdn.microsoft.com/ad8753ba-ad20-4122-b0f2-eb165f98db67">Device Properties</a>.

For a code example that implements the <b>OnPropertyValueChanged</b> method, see <a href="https://msdn.microsoft.com/b31500d6-a79d-4e6e-878e-6bd77055f1ad">Device Events</a>.




## -see-also




<a href="https://msdn.microsoft.com/76d3cd52-30bd-48b0-8adc-c23991a60d1b">IMMNotificationClient Interface</a>
 

 

