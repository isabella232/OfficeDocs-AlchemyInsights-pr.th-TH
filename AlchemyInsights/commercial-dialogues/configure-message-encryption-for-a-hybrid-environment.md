---
title: การกําหนดค่าการเข้ารหัสลับข้อความในสภาพแวดล้อมแบบไฮบริด
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
ms.openlocfilehash: 59360a040fe413e92cd880b1225b9006384a823f6e8abeb7ef922949b9a874fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035241"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>การกําหนดค่าการเข้ารหัสลับข้อความในสภาพแวดล้อมแบบไฮบริด

For hybrid Exchange environments, on-premises users can sended email using Office Message Encryption (OME) only if email is routed through Exchange Online.

เมื่อต้องการเข้ารหัสลับอีเมลโดยใช้ OME ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ใช้ตัวช่วยสร้าง [การกําหนดค่า](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) แบบไฮบริดเพื่อตั้งค่าสภาพแวดล้อมแบบไฮบริดของคุณ ไม่ต้องมีขั้นตอนพิเศษใด ๆ ในการตั้งค่าการเข้ารหัสลับ
2. [ตั้งค่ากฎของลโฟลว์จดหมายของคุณ](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) เพื่อการเข้ารหัสลับแบบที่คุณมักจะใช้ตามปกติ


