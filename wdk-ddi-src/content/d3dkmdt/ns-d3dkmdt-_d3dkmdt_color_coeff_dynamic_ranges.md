---
UID: NS:d3dkmdt._D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES
title: "_D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES"
author: windows-driver-content
description: The D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES contains values that indicate the dynamic range of each color channel of a video present target or a monitor.
old-location: display\d3dkmdt_color_coeff_dynamic_ranges.htm
tech.root: display
ms.assetid: 7fdd1d52-c406-4da7-adff-4300e795be00
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES, D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES structure [Display Devices], DmStructs_33f2d82d-dbb3-4d51-bc3c-5c8e334d5113.xml, _D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES, d3dkmdt/D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES, display.d3dkmdt_color_coeff_dynamic_ranges
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3dkmdt.h
req.include-header: D3dkmdt.h
req.target-type: Windows
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating systems.
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
-	HeaderDef
api_location:
-	d3dkmdt.h
api_name:
-	D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES
product:
- Windows
targetos: Windows
req.typenames: D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES
---

# _D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES structure


## -description


The D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES contains values that indicate the dynamic range of each color channel of a video present target or a monitor.


## -struct-fields




### -field FirstChannel

The bit depth of the first color channel.


### -field SecondChannel

The bit depth of the second color channel.


### -field ThirdChannel

The bit depth of the third color channel.


### -field FourthChannel

Reserved.


## -remarks



The <b>VidPnTargetColorCoeffDynamicRanges</b> member of the <a href="https://msdn.microsoft.com/library/windows/hardware/ff546647">D3DKMDT_VIDPN_PRESENT_PATH</a> structure is a D3DKMDT_COLOR_COEFF_DYNAMIC_RANGES structure.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff545984">D3DKMDT_COLOR_BASIS</a>
 

 

