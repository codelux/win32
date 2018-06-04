---
title: Bluetooth and WSALookupServiceNext
description: Bluetooth uses the WSALookupServiceNext function to match queries specified in a previous call to WSALookupServiceBegin.
ms.assetid: d43cf444-adb6-4313-9614-a8d6d868a88f
keywords:
- Bluetooth
- WSALookupServiceNext
- Bluetooth and WSALookupServiceNext
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Bluetooth and WSALookupServiceNext

Bluetooth uses the [**WSALookupServiceNext**](https://msdn.microsoft.com/library/windows/desktop/ms741641) function to match queries specified in a previous call to [**WSALookupServiceBegin**](https://msdn.microsoft.com/library/windows/desktop/ms741633). The results of the **WSALookupServiceNext** function are determined by settings set forth in the [**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679) structure passed in the initial **WSALookupServiceBegin** function call.

The steps for device inquiry and service discovery in Bluetooth are sufficiently different to merit separate treatment. For more information on Bluetooth and the [**WSALookupServiceBegin**](https://msdn.microsoft.com/library/windows/desktop/ms741633) function for device inquiries, see [Bluetooth and WSALookupServiceBegin for Device Inquiry](bluetooth-and-wsalookupservicebegin-for-device-inquiry.md). For more information on Bluetooth and the **WSALookupServiceBegin** function for service discovery, see [Bluetooth and WSALookupServiceBegin for Service Discovery](bluetooth-and-wsalookupservicebegin-for-service-discovery.md).

## Related topics

<dl> <dt>

[Discovering Bluetooth Devices and Services](discovering-bluetooth-devices-and-services.md)
</dt> <dt>

[Bluetooth and WSALookupServiceBegin for Device Inquiry](bluetooth-and-wsalookupservicebegin-for-device-inquiry.md)
</dt> <dt>

[Bluetooth and WSALookupServiceBegin for Service Discovery](bluetooth-and-wsalookupservicebegin-for-service-discovery.md)
</dt> <dt>

[Bluetooth and WSALookupServiceEnd](bluetooth-and-wsalookupserviceend.md)
</dt> <dt>

[**BTH\_QUERY\_SERVICE**](/windows/desktop/api/Ws2bth/ns-ws2bth-_bth_query_service)
</dt> <dt>

[**connect**](https://msdn.microsoft.com/library/windows/desktop/ms737625)
</dt> <dt>

[**SOCKADDR\_BTH**](/windows/desktop/api/Ws2bth/ns-ws2bth-_sockaddr_bth)
</dt> <dt>

[**WSALookupServiceBegin**](https://msdn.microsoft.com/library/windows/desktop/ms741633)
</dt> <dt>

[**WSALookupServiceEnd**](https://msdn.microsoft.com/library/windows/desktop/ms741637)
</dt> <dt>

[**WSALookupServiceNext**](https://msdn.microsoft.com/library/windows/desktop/ms741641)
</dt> <dt>

[**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679)
</dt> </dl>

 

 



