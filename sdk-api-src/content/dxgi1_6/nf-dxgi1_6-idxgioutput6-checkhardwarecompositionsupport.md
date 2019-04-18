---
UID: NF:dxgi1_6.IDXGIOutput6.CheckHardwareCompositionSupport
title: IDXGIOutput6::CheckHardwareCompositionSupport (dxgi1_6.h)
author: windows-sdk-content
description: Notifies applications that hardware stretching is supported.
old-location: direct3ddxgi\idxgioutput6_checkhardwarecompositionsupport.htm
tech.root: direct3ddxgi
ms.assetid: 1FFB01F3-9C12-41CE-9CF6-F130CC65A7DC
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CheckHardwareCompositionSupport, CheckHardwareCompositionSupport method [DXGI], CheckHardwareCompositionSupport method [DXGI],IDXGIOutput6 interface, IDXGIOutput6 interface [DXGI],CheckHardwareCompositionSupport method, IDXGIOutput6.CheckHardwareCompositionSupport, IDXGIOutput6::CheckHardwareCompositionSupport, direct3ddxgi.idxgioutput6_checkhardwarecompositionsupport, dxgi1_6/IDXGIOutput6::CheckHardwareCompositionSupport
ms.topic: method
req.header: dxgi1_6.h
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
req.lib: DXGI.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - DXGI.lib
 - DXGI.dll
api_name:
 - IDXGIOutput6.CheckHardwareCompositionSupport
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: RS5, 19H1
---

# IDXGIOutput6::CheckHardwareCompositionSupport


## -description


Notifies applications that hardware stretching is supported.


## -parameters




### -param pFlags [out]

Type: <b>UINT*</b>

A bitfield of <a href="https://msdn.microsoft.com/FA8BCF74-58CB-4806-A0A5-1D8E6EC576DC">DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS</a> enumeration values describing which types of hardware composition are supported. The values are bitwise OR'd together.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns a code that indicates success or failure.




## -see-also




<a href="https://msdn.microsoft.com/b561b26b-961c-4d5e-8483-56b51b989bf7">DXGI Interfaces</a>



<a href="https://msdn.microsoft.com/FA8BCF74-58CB-4806-A0A5-1D8E6EC576DC">DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS enumeration</a>



<a href="https://msdn.microsoft.com/2F04E7F1-8295-441B-9E86-65C3DE5DE75F">IDXGIOutput6 interface</a>
 

 

