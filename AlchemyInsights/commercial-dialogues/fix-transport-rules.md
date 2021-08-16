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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034773"
---
# <a name="fix-transport-rules"></a>แก้ไขกฎการส่งผ่าน

กฎลโฟลว์จดหมายแบบปรับแต่งเองจะมีผลต่อข้อความนี้ เมื่อต้องการตรวจทานกฎที่แน่นอน ให้ต่อไปนี้:

1. ในผลลัพธ์การส่ง ภายใต้ **ข้อมูลเพิ่มเติม** ให้สังเกต **GUID** หรือ **ชื่อ** นโยบาย
2. เปิดใช้ Exchange Management Shell For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. เรียกใช้สั่งนี้ (โดยใช้ GUID จากการส่งของคุณ):  **Get-TransportRule -identity "GUID" | fl * Description***
4. ตรวจทานรายละเอียดเพื่อดูเงื่อนไขที่กําหนดค่าแล้วซึ่งมีผลต่อข้อความ

เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดูที่ Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)
