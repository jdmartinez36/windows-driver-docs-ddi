---
UID: NS:ntddrilapitypes.RILMSGINSTATUS
title: RILMSGINSTATUS (ntddrilapitypes.h)
description: "Microsoft reserves the RILMSGINSTATUS structure for internal use only. Don't use this structure in your code."
old-location: netvista\rilmsginstatus.htm
tech.root: netvista
ms.date: 05/02/2018
keywords: ["RILMSGINSTATUS structure"]
ms.keywords: "*LPRILMSGINSTATUS, RILMSGINSTATUS, RILMSGINSTATUS structure [Network Drivers Starting with Windows Vista], netvista.rilmsginstatus, ntddrilapitypes/RILMSGINSTATUS"
req.header: ntddrilapitypes.h
req.include-header: Rilapitypes.h
req.target-type: Windows
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
targetos: Windows
req.typenames: RILMSGINSTATUS, *LPRILMSGINSTATUS
f1_keywords:
 - RILMSGINSTATUS
 - ntddrilapitypes/RILMSGINSTATUS
 - LPRILMSGINSTATUS
 - ntddrilapitypes/LPRILMSGINSTATUS
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ntddrilapitypes.h
api_name:
 - RILMSGINSTATUS
 - LPRILMSGINSTATUS
---

# RILMSGINSTATUS structure (ntddrilapitypes.h)


## -description

This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.

## -struct-fields

### -field dwMsgID

### -field raTgtRecipAddress

### -field stTgtSCReceiveTime

### -field stTgtDischargeTime

### -field dwReserved

### -field dwTgtDlvStatus

### -field dwProtocolID

### -field rmdDataCoding

### -field cbHdrLength

### -field cchMsgLength

### -field rgbHdr

### -field rgbMsg

