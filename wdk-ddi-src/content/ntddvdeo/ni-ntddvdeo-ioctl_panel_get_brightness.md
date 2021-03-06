---
UID: NI:ntddvdeo.IOCTL_PANEL_GET_BRIGHTNESS
title: IOCTL_PANEL_GET_BRIGHTNESS
author: windows-driver-content
description: Returns the brightness level for the display panel.
ms.assetid: 1bbd8248-a81a-40dd-972b-80b187da28da
ms.author: windowsdriverdev
ms.date:
ms.topic: ioctl
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: ntddvdeo.h
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
req.max-support:
topic_type:
-	apiref
api_type:
-	HeaderDef
api_location:
-	ntddvdeo.h
api_name:
-	IOCTL_PANEL_GET_BRIGHTNESS
product: 
- Windows
targetos: Windows
tech.root: display
---

# IOCTL_PANEL_GET_BRIGHTNESS IOCTL

## Major Code:  [[XREF-LINK:IRP_MJ_DEVICE_CONTROL]

## -description

Returns the brightness level for the display panel.

## -ioctlparameters

### -input-buffer



### -input-buffer-length



### -output-buffer



### -output-buffer-length



### -in-out-buffer



### -inout-buffer-length



### -status-block

Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.
Otherwise, Status to the appropriate error condition as a NTSTATUS code.


