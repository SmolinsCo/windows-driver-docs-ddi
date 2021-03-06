---
UID: NF:wdtf.IWDTFTarget2.get_Type
title: IWDTFTarget2::get_Type
author: windows-driver-content
description: Gets a value that identifies the depot that the target comes from.
old-location: dtf\iwdtftarget2_type.htm
tech.root: dtf
ms.assetid: 76b13505-7404-475c-98d8-fe3b3ed25720
ms.author: windowsdriverdev
ms.date: 4/4/2018
ms.keywords: IWDTFTarget2 interface [Windows Device Testing Framework],Type property, IWDTFTarget2.Type, IWDTFTarget2.get_Type, IWDTFTarget2::Type, IWDTFTarget2::get_Type, Microsoft.WDTF.IWDTFTarget2.Type, Microsoft::WDTF::IWDTFTarget2::Type, Type property [Windows Device Testing Framework], Type property [Windows Device Testing Framework],IWDTFTarget2 interface, dtf.iwdtftarget2_type, get_Type, wdtf/IWDTFTarget2::Type, wdtf/IWDTFTarget2::get_Type
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wdtf.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Professional
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WDTF.idl
req.max-support: 
req.namespace: Microsoft.WDTF
req.assembly: WDTF.Interop.metadata_dll
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
-	WDTF.Interop.metadata_dll.dll
api_name:
-	IWDTFTarget2.Type
-	IWDTFTarget2.get_Type
product:
- Windows
targetos: Windows
req.typenames: 
---

# IWDTFTarget2::get_Type


## -description


Gets a value that identifies the depot that the target comes from.

This property is read-only.


## -parameters


## -remarks



The value can be one of the following:

<ul>
<li>
<b>Device</b> if the target comes from the 
<a href="https://msdn.microsoft.com/library/windows/hardware/hh406391">IWDTFDeviceDepot2</a> interface.

</li>
<li>
<b>System</b> if the target comes from the 
<a href="https://msdn.microsoft.com/library/windows/hardware/hh439331">IWDTFSystemDepot2</a> interface.

</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/hh406391">IWDTFDeviceDepot2</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/hh439331">IWDTFSystemDepot2</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/hh439367">IWDTFTarget2</a>
 

 

