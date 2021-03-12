---
title: แก้ไขกฎการส่งผ่าน
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750572"
---
# <a name="fix-transport-rules"></a>แก้ไขกฎการส่งผ่าน

กฎล>ล.ย.จดหมายแบบปรับแต่งเองมีผลต่อข้อความนี้ เมื่อต้องการตรวจทานกฎที่แน่นอน ให้ทต่อไปนี้:

1. ในผลลัพธ์การส่ง **ภายใต้ข้อมูลเพิ่มเติม ให้** จด **GUID** หรือ **ชื่อ** นโยบาย
2. เปิดใช้ Exchange Management Shell For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. เรียกใช้การสั่งนี้ (โดยใช้ GUID จากการส่งของคุณ):  **Get-TransportRule -identity "GUID" | fl * Description***
4. ตรวจทานรายละเอียดเพื่อดูเงื่อนไขที่กําหนดค่าแล้วที่ได้รับผลกระทบในข้อความ

เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)
