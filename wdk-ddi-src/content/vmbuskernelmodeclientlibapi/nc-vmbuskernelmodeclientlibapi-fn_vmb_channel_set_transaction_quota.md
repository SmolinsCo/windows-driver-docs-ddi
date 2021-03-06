---
UID: NC:vmbuskernelmodeclientlibapi.FN_VMB_CHANNEL_SET_TRANSACTION_QUOTA
title: FN_VMB_CHANNEL_SET_TRANSACTION_QUOTA
author: windows-driver-content
description: The VmbChannelSetTransactionQuota function sets the incoming packet quota.
tech.root: netvista
ms.assetid: a5e56060-b5b9-4d65-8808-1d4a430521fa
ms.author: windowsdriverdev
ms.date: 05/22/2018
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: vmbuskernelmodeclientlibapi.h
req.include-header:
req.target-type:
req.target-min-winverclnt: Windows 10, version 1803
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
-	vmbuskernelmodeclientlibapi.h
api_name: 
-	FN_VMB_CHANNEL_SET_TRANSACTION_QUOTA
product:
-	Windows
targetos: Windows
---

# FN_VMB_CHANNEL_SET_TRANSACTION_QUOTA callback function

## -description

<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

The <b>VmbChannelSetTransactionQuota</b> function sets the incoming packet quota.

## -prototype

```
//Declaration

FN_VMB_CHANNEL_SET_TRANSACTION_QUOTA FnVmbChannelSetTransactionQuota; 

// Definition

VOID FnVmbChannelSetTransactionQuota 
(
	VMBCHANNEL Channel
	UINT32 Quota
)
{...}

```

## -parameters

### -param Channel

A handle for a channel.  

### -param Quota: 

 The maximum outstanding packet quota. This value must be greater than 0.

## -returns

This function does not return a value.

## -remarks

The incoming packet quota can be set to be lower than the current
outstanding packet count. In that case, no new packets are removed from
the queue until sufficient packets have been completed.


 If the queue is currently blocked due to quota, this operation does not restart it. The queue only restarts once a packet is completed.

> [!IMPORTANT]
> This function is called through the VMBus Kernel Mode Client Library (KMCL) interface, provided by the Vmbkmcl.sys bus driver. 
>
> To access the KMCL interface, allocate a **KMCL_CLIENT_INTERFACE_V1** structure to receive the interface, then call either [**WdfFdoQueryForInterface**](../wdffdo/nf-wdffdo-wdffdoqueryforinterface.md) or [**WdfIoTargetQueryForInterface**](../wdfiotarget/nf-wdfiotarget-wdfiotargetqueryforinterface.md) with these parameters:
> 
> - *InterfaceType* parameter: **KMCL_CLIENT_INTERFACE_TYPE**
> - *Size* parameter: `sizeof(KMCL_CLIENT_INTERFACE_V1)`
> - *Version* parameter: **KMCL_CLIENT_INTERFACE_VERSION_LATEST** 
>
> If the interface query function succeeds, the **KMCL_CLIENT_INTERFACE_V1** structure contains function pointers for the VMBus KMCL functions that you can use to call them.
>
> For more information about driver-defined interfaces, see [Using Driver-Defined Interfaces](https://docs.microsoft.com/windows-hardware/drivers/wdf/using-driver-defined-interfaces).

## -see-also
