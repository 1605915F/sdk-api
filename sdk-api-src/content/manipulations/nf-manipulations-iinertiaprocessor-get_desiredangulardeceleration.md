---
UID: NF:manipulations.IInertiaProcessor.get_DesiredAngularDeceleration
title: IInertiaProcessor::get_DesiredAngularDeceleration (manipulations.h)
author: windows-sdk-content
description: The DesiredAngularDeceleration property specifies the desired rate that the target object will stop spinning in radians per msec squared.
old-location: wintouch\iinertiaprocessor_desiredangulardeceleration.htm
tech.root: wintouch
ms.assetid: ee3bb3c8-4d7d-424b-abc9-db7307793794
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DesiredAngularDeceleration property [Windows Touch], DesiredAngularDeceleration property [Windows Touch],IInertiaProcessor interface, IInertiaProcessor interface [Windows Touch],DesiredAngularDeceleration property, IInertiaProcessor.DesiredAngularDeceleration, IInertiaProcessor.get_DesiredAngularDeceleration, IInertiaProcessor::DesiredAngularDeceleration, IInertiaProcessor::get_DesiredAngularDeceleration, IInertiaProcessor::put_DesiredAngularDeceleration, get_DesiredAngularDeceleration, manipulations/IInertiaProcessor::DesiredAngularDeceleration, manipulations/IInertiaProcessor::get_DesiredAngularDeceleration, manipulations/IInertiaProcessor::put_DesiredAngularDeceleration, wintouch.iinertiaprocessor_desiredangulardeceleration
ms.topic: method
req.header: manipulations.h
req.include-header: Manipulations.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - manipulations.h
api_name:
 - IInertiaProcessor.DesiredAngularDeceleration
 - IInertiaProcessor.get_DesiredAngularDeceleration
 - IInertiaProcessor.put_DesiredAngularDeceleration
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInertiaProcessor::get_DesiredAngularDeceleration


## -description


The <b>DesiredAngularDeceleration</b> property specifies the desired rate that the target object will stop spinning in radians per  msec squared.

This property is read/write.


## -parameters


## -remarks



<b>DesiredAngularDeceleration</b> and <a href="https://msdn.microsoft.com/42fcda66-8992-4a44-b4d5-04d4f2c7e25a">DesiredRotation</a> are mutually exclusive.  If one is set, the other should be NaN.
		

If inertia processing has already started, setting <b>DesiredAngularDeceleration</b> will reset the inertia engine to the initial state with new deceleration value applied.
      

Call this function to set the initial state of inertia. You would call this function most likely during the <a href="https://msdn.microsoft.com/1284df32-f4e8-43b3-b825-9172ad39f0e6">ManipulationCompleted</a> event of the <a href="https://msdn.microsoft.com/963f87c1-e128-4bd5-9f28-d49418f768fb">IManipulationProcessor</a> or in the constructor of the <a href="https://msdn.microsoft.com/8dc171eb-0c6e-41dd-b506-5f91ea703a53">IInertiaProcessor</a> interface.




## -see-also




<a href="https://msdn.microsoft.com/42fcda66-8992-4a44-b4d5-04d4f2c7e25a">DesiredRotation</a>



<a href="https://msdn.microsoft.com/3261b461-add2-4e92-9a51-b2d46630fb4f">Handling Inertia in Unmanaged Code</a>



<a href="https://msdn.microsoft.com/8dc171eb-0c6e-41dd-b506-5f91ea703a53">IInertiaProcessor</a>



<a href="https://msdn.microsoft.com/188b6936-b36e-4e57-9118-8b61ed134c17">Inertia Mechanics</a>



<a href="https://msdn.microsoft.com/a15ac600-ef03-4234-ac38-dc3cf212a3cb">InitialAngularVelocity</a>



<a href="https://msdn.microsoft.com/47fd1a49-8e14-4076-8ce6-f0c4917e8cf1">Properties</a>
 

 

