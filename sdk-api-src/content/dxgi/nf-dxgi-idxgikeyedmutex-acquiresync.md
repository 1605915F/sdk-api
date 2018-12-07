---
UID: NF:dxgi.IDXGIKeyedMutex.AcquireSync
title: IDXGIKeyedMutex::AcquireSync
author: windows-sdk-content
description: Using a key, acquires exclusive rendering access to a shared resource.
old-location: direct3ddxgi\idxgikeyedmutex_acquiresync.htm
tech.root: direct3ddxgi
ms.assetid: 31edab76-7b16-4a02-83ff-998c21e77f2e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 06d995ac-16d4-215c-4d9a-179636a32853, AcquireSync, AcquireSync method [DXGI], AcquireSync method [DXGI],IDXGIKeyedMutex interface, IDXGIKeyedMutex interface [DXGI],AcquireSync method, IDXGIKeyedMutex.AcquireSync, IDXGIKeyedMutex::AcquireSync, direct3ddxgi.idxgikeyedmutex_acquiresync, dxgi/IDXGIKeyedMutex::AcquireSync
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dxgi.h
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
 - IDXGIKeyedMutex.AcquireSync
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIKeyedMutex::AcquireSync


## -description


Using a key, acquires exclusive rendering access to a shared resource.


## -parameters




### -param Key

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT64</a></b>

A value that indicates which device to give access to. This method will succeed when the device that currently owns the surface calls 
          the <a href="https://msdn.microsoft.com/324741c9-33f2-4420-8c3f-4984e2ca0962">IDXGIKeyedMutex::ReleaseSync</a> method using the same value. This value can be any UINT64 value.


### -param dwMilliseconds

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

The time-out interval, in milliseconds. This method will return if the interval elapses, and the keyed mutex has not been released  using the specified <i>Key</i>. 
          If this value is set to zero, the <b>AcquireSync</b> method will test to see if the keyed mutex has been released and returns immediately. 
          If this value is set to INFINITE, the time-out interval will never elapse.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Return S_OK if successful.

If the owning device attempted to create another keyed mutex on the same shared resource, <b>AcquireSync</b> returns E_FAIL.

<b>AcquireSync</b> can also return the following <a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a> constants. Therefore, you should explicitly check for these constants. If you only use the <a href="https://msdn.microsoft.com/7a258b0b-d214-46c5-be0a-6493cd14a0e5">SUCCEEDED</a> macro on the return value to determine if  <b>AcquireSync</b> succeeded, you will not catch these constants.

<ul>
<li>WAIT_ABANDONED - The shared surface and keyed mutex are no longer in a consistent state. 
        If <b>AcquireSync</b> returns this value, you should release and recreate both the keyed mutex and the shared surface.</li>
<li>WAIT_TIMEOUT - The time-out interval elapsed before the specified key was released.</li>
</ul>



## -remarks



The <b>AcquireSync</b> method creates a lock to a surface that is shared between multiple devices, allowing only one device to render to a surface at a time.  
      This method uses a key to determine which device currently has exclusive access to the surface.

When a surface is created using the <b>D3D10_RESOURCE_MISC_SHARED_KEYEDMUTEX</b> value of the <a href="https://msdn.microsoft.com/en-us/library/Bb172412(v=VS.85).aspx">D3D10_RESOURCE_MISC_FLAG</a> enumeration, 
      you must call the <b>AcquireSync</b> method before rendering to the surface.  You must call the <a href="https://msdn.microsoft.com/324741c9-33f2-4420-8c3f-4984e2ca0962">ReleaseSync</a> method when you are done 
      rendering to a surface.

To acquire a reference to the keyed mutex object of a shared resource, call the <a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">QueryInterface</a> method of the resource and pass in 
      the <b>UUID</b> of the <a href="https://msdn.microsoft.com/f790eb46-f116-4258-8c8d-de1ece4a1f21">IDXGIKeyedMutex</a> interface.  For more information about acquiring this reference, see the following code example.

The <b>AcquireSync</b> method uses the key as follows, depending on the state of the surface:

<ul>
<li>On initial creation, the surface is unowned and any device can call the <b>AcquireSync</b> method to gain access. 
        For an unowned device, only a key of 0 will succeed. Calling the <b>AcquireSync</b> method for any other key will stall the 
        calling CPU thread.</li>
<li>If the surface is owned by a device when you call the <b>AcquireSync</b> method, the CPU thread that called 
        the <b>AcquireSync</b> method will stall until the owning device calls the <a href="https://msdn.microsoft.com/324741c9-33f2-4420-8c3f-4984e2ca0962">ReleaseSync</a> method 
        using the same Key.</li>
<li>If the surface is unowned when you call the <b>AcquireSync</b> method (for example, the last owning device has already called 
        the <a href="https://msdn.microsoft.com/324741c9-33f2-4420-8c3f-4984e2ca0962">ReleaseSync</a> method), the <b>AcquireSync</b> method will succeed if you specify the same key 
        that was specified when the <b>ReleaseSync</b> method was last called. Calling the <b>AcquireSync</b> 
          method using  any other key will cause a stall.</li>
<li>When the owning device calls the <a href="https://msdn.microsoft.com/324741c9-33f2-4420-8c3f-4984e2ca0962">ReleaseSync</a> method with a particular key, and more than one device is waiting after 
        calling the  <b>AcquireSync</b> method using the same key, any one of the waiting devices could be woken up first. 
        The order in which devices are woken up is undefined.</li>
<li>A keyed mutex does not support recursive calls to the <b>AcquireSync</b> method.</li>
</ul>

#### Examples

<b>Acquiring a Keyed Mutex</b>

The following code example demonstrates how to acquire a lock to a shared resource and how to specify a key upon release.


```

// pDesc has already been set up with texture description.
pDesc.MiscFlags = D3D10_RESOURCE_MISC_SHARED_KEYEDMUTEX;

// Create a shared texture resource.
pD3D10DeviceD->CreateTexture2D(pDesc, NULL, pD3D10Texture);

// Acquire a reference to the keyed mutex.
pD3D10Texture->QueryInterface(_uuidof(IDXGIKeyedMutex), pDXGIKeyedMutex);

// Acquire a lock to the resource.
pDXGIKeyedMutex->AcquireSync(0, INFINITE);

// Release the lock and specify a key.
pDXGIKeyedMutex->ReleaseSync(1);
          
```


<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/b561b26b-961c-4d5e-8483-56b51b989bf7">DXGI Interfaces</a>



<a href="https://msdn.microsoft.com/f790eb46-f116-4258-8c8d-de1ece4a1f21">IDXGIKeyedMutex</a>



<a href="https://msdn.microsoft.com/324741c9-33f2-4420-8c3f-4984e2ca0962">IDXGIKeyedMutex::ReleaseSync</a>
 

 

