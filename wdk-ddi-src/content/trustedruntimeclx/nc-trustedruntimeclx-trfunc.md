---
UID: NC:trustedruntimeclx.TRFUNC
title: TRFUNC
author: windows-driver-content
description: 
ms.assetid: 8e25c958-8de1-4ae5-ace9-91184e90a1bd
ms.author: windowsdriverdev
ms.date: 
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: trustedruntimeclx.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
topic_type: 
-	apiref
api_type: 
-	UserDefined
api_location: 
-	trustedruntimeclx.h
api_name: 
-	TRFUNC
product:
-	Windows
targetos: Windows
---

# TRFUNC callback function

## -description

Implemented by the client driver to ... 

## -prototype

```
//Declaration

TRFUNC Trfunc; 

// Definition

VOID Trfunc 
(
	VOID Arg1
)
{...}

```

## -parameters

### -param Arg1: 



## -returns

Returns VOID that ...

## -remarks

Register your implementation of this callback function by setting the appropriate member of <!-- REPLACE ME --> and then calling <!-- REPLACE ME -->.


## -see-also