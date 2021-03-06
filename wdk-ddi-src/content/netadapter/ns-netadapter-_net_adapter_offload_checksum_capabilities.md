---
UID: NS:netadapter._NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES
title: _NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES
author: windows-driver-content
description: The NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES structure describes a network interface card (NIC)'s capabilities for offloading checksum calculation and validation.
tech.root: netvista
ms.assetid: edf69542-3428-4919-ac04-872429a873d8
ms.author: windowsdriverdev
ms.date: 07/19/2018
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES, NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES, *PNET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES, 
req.header: netadapter.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver: 1.27
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES, *PNET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	netadapter.h
api_name: 
-	_NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES
product:
- Windows
targetos: Windows
---

# _NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES structure

## -description

> [!WARNING]
> Some information in this topic relates to prereleased product, which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.
>
> NetAdapterCx is preview only in Windows 10, version 1809.

The **NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES** structure describes a network interface card (NIC)'s capabilities for offloading checksum calculation and validation.

## -struct-fields

### -field Size

The size of this structure, in bytes.
 
### -field IPv4

A flag specifying whether the NIC can calculate and validate IPv4 checksum.
 
### -field Tcp

A flag specifying whether the NIC can calculate and validate TCP checksum.
 
### -field Udp
 
A flag specifying whether the NIC can calculate and validate UDP checksum.

## -remarks

Call [**NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES_INIT**](nf-netadapter-net_adapter_offload_checksum_capabilities_init.md) to initialize this structure. An initialized **NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES** structure is passed as a parameter to [**NetAdapterOffloadSetChecksumCapabilities**](nf-netadapter-netadapteroffloadsetchecksumcapabilities.md).

## -see-also

[NetAdapterCx hardware offloads](https://docs.microsoft.com/windows-hardware/drivers/netcx/netadaptercx-hardware-offloads)

[**NET_ADAPTER_OFFLOAD_CHECKSUM_CAPABILITIES_INIT**](nf-netadapter-net_adapter_offload_checksum_capabilities_init.md)

[**NetAdapterOffloadSetChecksumCapabilities**](nf-netadapter-netadapteroffloadsetchecksumcapabilities.md)
