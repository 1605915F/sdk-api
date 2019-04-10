---
UID: NF:manipulations.IInertiaProcessor.put_InitialVelocityY
title: IInertiaProcessor::put_InitialVelocityY (manipulations.h)
author: windows-sdk-content
description: The InitialVelocityY property specifies the initial movement of the target object on the vertical axis.
old-location: wintouch\iinertiaprocessor_initialvelocityy.htm
tech.root: wintouch
ms.assetid: 3ba0aa0c-a819-4833-883b-218702052ce1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IInertiaProcessor interface [Windows Touch],InitialVelocityY property, IInertiaProcessor.InitialVelocityY, IInertiaProcessor.put_InitialVelocityY, IInertiaProcessor::InitialVelocityY, IInertiaProcessor::get_InitialVelocityY, IInertiaProcessor::put_InitialVelocityY, InitialVelocityY property [Windows Touch], InitialVelocityY property [Windows Touch],IInertiaProcessor interface, manipulations/IInertiaProcessor::InitialVelocityY, manipulations/IInertiaProcessor::get_InitialVelocityY, manipulations/IInertiaProcessor::put_InitialVelocityY, put_InitialVelocityY, wintouch.iinertiaprocessor_initialvelocityy
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
 - IInertiaProcessor.InitialVelocityY
 - IInertiaProcessor.get_InitialVelocityY
 - IInertiaProcessor.put_InitialVelocityY
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInertiaProcessor::put_InitialVelocityY


## -description


The <b>InitialVelocityY</b> property specifies the initial movement of the target object on the vertical axis.

This property is read/write.


## -parameters


## -remarks



If inertia processing has already started, setting <b>InitialVelocityY</b> will reset the inertia engine to the initial state with new velocity values applied.		
		

Call this function to set the initial state of inertia. You would call this function most likely during the <a href="https://msdn.microsoft.com/1284df32-f4e8-43b3-b825-9172ad39f0e6">ManipulationCompleted</a> event of the <a href="https://msdn.microsoft.com/963f87c1-e128-4bd5-9f28-d49418f768fb">IManipulationProcessor</a> or in the constructor of the <a href="https://msdn.microsoft.com/8dc171eb-0c6e-41dd-b506-5f91ea703a53">IInertiaProcessor</a> interface.




## -see-also




<a href="https://msdn.microsoft.com/b531c4e5-8437-4869-9264-3fe131b8acc8">GetVelocityY</a>



<a href="https://msdn.microsoft.com/3261b461-add2-4e92-9a51-b2d46630fb4f">Handling Inertia in Unmanaged Code</a>



<a href="https://msdn.microsoft.com/8dc171eb-0c6e-41dd-b506-5f91ea703a53">IInertiaProcessor</a>



<a href="https://msdn.microsoft.com/188b6936-b36e-4e57-9118-8b61ed134c17">Inertia Mechanics</a>



<a href="https://msdn.microsoft.com/23ae7083-0a78-4628-8a04-f9bd762aac02">InitialVelocityX</a>



<a href="https://msdn.microsoft.com/47fd1a49-8e14-4076-8ce6-f0c4917e8cf1">Properties</a>
 

 

