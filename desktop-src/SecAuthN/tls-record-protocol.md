---
Description: The Transport Layer Security (TLS) Record protocol secures application data using the keys created during the Handshake.
ms.assetid: 3ad4cbd9-ce7c-4882-9c53-c935068c0ba7
title: TLS Record Protocol
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# TLS Record Protocol

The [*Transport Layer Security*](https://www.bing.com/search?q=*Transport Layer Security*) (TLS) Record protocol secures application data using the keys created during the [Handshake](tls-handshake-protocol.md). The Record Protocol is responsible for securing application data and verifying its [*integrity*](https://www.bing.com/search?q=*integrity*) and origin. It manages the following:

-   Dividing outgoing messages into manageable blocks, and reassembling incoming messages.
-   Compressing outgoing blocks and decompressing incoming blocks (optional).
-   Applying a [*Message Authentication Code*](https://www.bing.com/search?q=*Message Authentication Code*) (MAC) to outgoing messages, and verifying incoming messages using the MAC.
-   Encrypting outgoing messages and decrypting incoming messages.

When the Record Protocol is complete, the outgoing encrypted data is passed down to the Transmission Control Protocol (TCP) layer for transport.

 

 


