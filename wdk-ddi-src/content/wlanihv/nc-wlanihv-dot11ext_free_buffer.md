---
UID: NC:wlanihv.DOT11EXT_FREE_BUFFER
title: DOT11EXT_FREE_BUFFER (wlanihv.h)
description: The DOT11EXT_FREE_BUFFER callback function is part of the Native 802.11 Wireless LAN interface, which is deprecated for Windows 10 and later.
old-location: netvista\dot11extfreebuffer.htm
tech.root: netvista
ms.date: 02/16/2018
keywords: ["DOT11EXT_FREE_BUFFER callback"]
ms.keywords: DOT11EXT_FREE_BUFFER, Dot11ExtFreeBuffer, Dot11ExtFreeBuffer callback function [Network Drivers Starting with Windows Vista], Native_802.11_IHV_Ext_af721540-28a8-43c2-a649-ce0f6fb9adce.xml, netvista.dot11extfreebuffer, wlanihv/Dot11ExtFreeBuffer
req.header: wlanihv.h
req.include-header: Wlanihv.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating   systems.
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
req.typenames: DRIVER_INFO_8W, *PDRIVER_INFO_8W, *LPDRIVER_INFO_8W
req.product: Windows 10 or later.
f1_keywords:
 - DOT11EXT_FREE_BUFFER
 - wlanihv/DOT11EXT_FREE_BUFFER
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - wlanihv.h
api_name:
 - DOT11EXT_FREE_BUFFER
---

# DOT11EXT_FREE_BUFFER callback


## -description

<div class="alert"><b>Important</b>  The <a href="/previous-versions/windows/hardware/wireless/ff560689(v=vs.85)">Native 802.11 Wireless LAN</a> interface is deprecated in Windows 10 and later. Please use the WLAN Device Driver Interface (WDI) instead. For more information about WDI, see <a href="/windows-hardware/drivers/network/wifi-universal-driver-model">WLAN Universal Windows driver model</a>.</div><div> </div>The IHV Extensions DLL calls the
  <b>Dot11ExtFreeBuffer</b> function to free memory allocated through a call to
  <a href="..\wlanihv\nc-wlanihv-dot11ext_allocate_buffer.md">Dot11ExtAllocateBuffer</a>.

## -parameters

### -param pvMemory 

[in, optional]
A pointer to the buffer to be freed. If the value of
     <i>pvMemory</i> is <b>NULL</b>, the
     <b>Dot11ExtFreeBuffer</b> function returns immediately.

## -prototype

```cpp
VOID WINAPI * Dot11ExtFreeBuffer(
  _In_opt_ LPVOID pvMemory
);
```

## -remarks

The IHV Extension DLL must not call the
    <b>Dot11ExtFreeBuffer</b> function for any variable-length buffer allocated
    within an IHV handler function and passed to the operating system through a parameter to the function. In
    this situation, the operating system is responsible for freeing the buffer after the return of the IHV
    Handler function.

For more information about the IHV Handler functions, see
    <a href="/windows-hardware/drivers/network/native-802-11-ihv-handler-functions">Native 802.11 IHV Handler
    Functions</a>.

## -see-also

<a href="/windows-hardware/drivers/network/native-802-11-ihv-handler-functions">Native 802.11 IHV Handler
   Functions</a>



<a href="..\wlanihv\nc-wlanihv-dot11ext_allocate_buffer.md">Dot11ExtAllocateBuffer</a>

