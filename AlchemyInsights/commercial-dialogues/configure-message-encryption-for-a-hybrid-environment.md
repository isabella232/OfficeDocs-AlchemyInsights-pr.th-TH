---
title: กําหนดค่าการเข้ารหัสลับข้อความในสภาพแวดล้อมแบบไฮบริด
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747946"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>กําหนดค่าการเข้ารหัสลับข้อความในสภาพแวดล้อมแบบไฮบริด

For hybrid Exchange environments, on-premises users can sended email using Office Message Encryption (OME) only if email is routed through Exchange Online.

เมื่อต้องการเข้ารหัสลับอีเมลโดยใช้ OME ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ใช้ตัวช่วยสร้าง [การกําหนดค่า](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) แบบไฮบริดเพื่อตั้งค่าสภาพแวดล้อมแบบไฮบริดของคุณ ไม่ต้องมีขั้นตอนพิเศษในการตั้งค่าการเข้ารหัสลับ
2. [ตั้งค่ากฎของลโฟลว์จดหมายของคุณ](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) การเข้ารหัสลับแบบที่คุณมักจะใช้ตามปกติ


