---
title: ปรับใช้หลักปฏิบัติที่ดีที่สุดกับคิวรีการค้นหาขั้นสูงในการหาข้อมูล
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696081"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>ปรับใช้หลักปฏิบัติที่ดีที่สุดกับคิวรีการค้นหาขั้นสูงในการหาข้อมูล

เมื่อต้องการให้ผลลัพธ์เร็วขึ้นและหลีกเลี่ยงการหมดเวลาขณะใช้งานคิวรีที่ซับซ้อน ให้ปรับใช้หลักปฏิบัติที่ดีที่สุดเหล่านี้:

- เมื่อลองคิวรีใหม่ ให้ใช้ขีดจํากัดเสมอเพื่อหลีกเลี่ยงชุดผลลัพธ์ที่มีขนาดใหญ่มาก นอกจากนี้ `count` ยังใช้สร้างแบบประเมินเริ่มต้นของขนาดของชุดผลลัพธ์
- ใช้ตัวกรองเวลาก่อน ให้จํากัดคิวรีของคุณสูงสุดเจ็ดวัน
- ในจุดเริ่มต้นของคิวรี หลังตัวกรองเวลา ให้เพิ่มตัวกรองที่คาดว่าจะเอาข้อมูลส่วนใหญ่ออก
- เมื่อค้นหาโทเค็นแบบเต็ม ให้ใช้ตัว `has` ตัวการ `contains` แทน
- เรียกใช้การค้นหาในคอลัมน์ใดคอลัมน์หนึ่งแทนที่จะเรียกใช้ในคอลัมน์ทั้งหมด
- เมื่อรวมตาราง ก่อนอื่นให้ระบุตารางที่มีแถวน้อยกว่า
- `project` เฉพาะคอลัมน์ที่จําเป็นจากตารางที่คุณได้รวมเข้าด้วยกัน

To learn more, see [Advanced query practices best](https://go.microsoft.com/fwlink/?linkid=2144812).
