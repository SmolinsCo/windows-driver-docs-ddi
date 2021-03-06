---
UID: NS:wwan._WWAN_MODEM_CONFIG_ID
title: _WWAN_MODEM_CONFIG_ID
author: windows-driver-content
description: The WWAN_MODEM_CONFIG_ID structure represents a unique ID for a modem configuration file.
tech.root: netvista
ms.assetid: e5653619-58fe-4fc7-a1d3-550a8cd6a735
ms.author: windowsdriverdev
ms.date: 03/23/2018
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _WWAN_MODEM_CONFIG_ID, *PWWAN_MODEM_CONFIG_ID, WWAN_MODEM_CONFIG_ID, 
req.header: wwan.h
req.include-header: wwan.h
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: WWAN_MODEM_CONFIG_ID, *PWWAN_MODEM_CONFIG_ID
topictype: 
-	apiref
apitype: 
-	HeaderDef
apilocation: 
-	wwan.h
apiname: 
-	_WWAN_MODEM_CONFIG_ID
product:
-	Windows
targetos: Windows
---

# _WWAN_MODEM_CONFIG_ID structure

## -description

The **WWAN_MODEM_CONFIG_ID** structure represents a unique ID for a modem configuration file.

## -struct-fields

### -field ConfigIdLen
A DWORD value indicating the length of **ConfigId**.
 
### -field ConfigId
A byte array representing the configuration ID. The maximum length of this field is 256 bits, or 32 bytes.

## -remarks
A value of **0** for **ConfigId** is a special value that indicates that the configuration ID is not available.

## -see-also

[WWAN_MODEM_CONFIG_INFO](ns-wwan-_wwan_modem_config_info.md)
