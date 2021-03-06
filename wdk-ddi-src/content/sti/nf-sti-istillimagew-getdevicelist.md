---
UID: NF:sti.IStillImageW.GetDeviceList
title: IStillImageW::GetDeviceList
author: windows-driver-content
description: The IStillImage::GetDeviceList method returns hardware characteristics for all installed still image devices.
old-location: image\istillimage_getdevicelist.htm
tech.root: image
ms.assetid: 43c8a5d2-7f34-4b68-b316-020049e98444
ms.author: windowsdriverdev
ms.date: 5/3/2018
ms.keywords: GetDeviceList, GetDeviceList method [Imaging Devices], GetDeviceList method [Imaging Devices],IStillImageW interface, IStillImageW interface [Imaging Devices],GetDeviceList method, IStillImageW.GetDeviceList, IStillImageW::GetDeviceList, image.istillimage_getdevicelist, sti/IStillImageW::GetDeviceList, stifnc_eb4712d7-33b5-40d3-87f9-6f5eef639039.xml
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: sti.h
req.include-header: Sti.h
req.target-type: Desktop
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
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	sti.h
api_name:
-	IStillImageW.GetDeviceList
product:
- Windows
targetos: Windows
req.typenames: 
---

# IStillImageW::GetDeviceList


## -description


The <b>IStillImage::GetDeviceList</b> method returns hardware characteristics for all installed still image devices.


## -parameters




### -param dwType

Reserved parameter, use <b>NULL</b>.


### -param dwFlags

Reserved parameter, use <b>NULL</b>.


### -param pdwItemsReturned [out]

Receives the number of STI_DEVICE_INFORMATION structures supplied in the buffer referenced by <i>ppBuffer</i>.


### -param ppBuffer [out]

Receives a handle to an STI-allocated buffer. This buffer will contain an array of <a href="https://msdn.microsoft.com/library/windows/hardware/ff548361">STI_DEVICE_INFORMATION</a> structures.


## -returns



If the operation succeeds, the method returns S_OK. Otherwise, it returns one of the STIERR-prefixed error codes defined in <i>stierr.h</i>.




## -remarks



The <b>IStillImage::GetDeviceList</b> method returns an <a href="https://msdn.microsoft.com/library/windows/hardware/ff548361">STI_DEVICE_INFORMATION</a> structure for each installed still-image device. Structure contents are typically used for creating user interface displays and for finding a device's internal name.

Before calling <b>IStillImage::GetDeviceList</b>, clients of the <b>IStillImage</b> COM interface must call <a href="https://msdn.microsoft.com/library/windows/hardware/ff543804">IStillImage::StiCreateInstance</a> to obtain an <b>IStillImage</b> interface pointer.

When the caller has finished using the array of STI_DEVICE_INFORMATION structures referenced by <i>ppBuffer</i>, it must deallocate the array by calling <b>LocalFree</b> (described in the Microsoft Windows SDK documentation).




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff543782">IStillImage::GetDeviceInfo</a>



<a href="https://msdn.microsoft.com/a9ceee48-cbb5-4448-83b4-9c19fe89fcb9">IStillImageW</a>
 

 

