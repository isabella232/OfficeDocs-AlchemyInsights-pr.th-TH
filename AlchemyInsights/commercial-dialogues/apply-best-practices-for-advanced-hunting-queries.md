---
title: ใช้หลักปฏิบัติที่ดีที่สุดกับคิวรีการหาคิวรีขั้นสูง
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930152"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>ใช้หลักปฏิบัติที่ดีที่สุดกับคิวรีการหาคิวรีขั้นสูง

เมื่อต้องการให้ผลลัพธ์เร็วขึ้นและเพื่อหลีกเลี่ยงการหมดเวลาขณะเรียกใช้คิวรีที่ซับซ้อน ให้ปรับใช้หลักปฏิบัติที่ดีที่สุดเหล่านี้:

- เมื่อลองคิวรีใหม่ ให้ใช้ขีดจํากัดเสมอเพื่อหลีกเลี่ยงการชุดผลลัพธ์ที่มีขนาดใหญ่มาก Also, `count` use to make an initial assessment of the result set's size.
- ใช้ตัวกรองเวลาก่อน ให้เหมาะที่จะจํากัดคิวรีของคุณไว้ไม่เกิน 7 วัน
- ในตอนต้นของคิวรี ให้เพิ่มตัวกรองเวลาที่ต้องการเอาข้อมูลส่วนใหญ่ออกทันที
- เมื่อค้นหาโทเค็นแบบเต็ม ให้ใช้ `has` ตัวตัวการแทน `contains`
- เรียกใช้การค้นหาในคอลัมน์ใดคอลัมน์หนึ่งแทนการค้นหาในคอลัมน์ทั้งหมด
- เมื่อรวมตาราง ก่อนอื่นให้ระบุตารางที่มีแถวน้อยกว่า
- `project` เฉพาะคอลัมน์ที่จําเป็นจากตารางที่คุณเข้าร่วม

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู หลักปฏิบัติที่ดีที่สุดของ [คิวรีการหาข้อมูล](https://go.microsoft.com/fwlink/?linkid=2144812)ขั้นสูง
