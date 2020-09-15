---
title: 'AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: 811a48587272776c8ece5e654a921c15cf52af5f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696567"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้

ถ้าคุณพบปัญหาเกี่ยวกับการทำเครื่องหมายการแสดงผลที่ไม่แสดงตามที่คาดไว้ให้ดูแนวทางต่อไปนี้:

1. ตรวจสอบให้แน่ใจว่าคุณได้รับการตรวจทาน[เมื่อมีการนำเครื่องหมายภาพไปใช้](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. สำหรับการติดป้าย Office ให้ตรวจทาน[เมื่อ office ๓๖๕ใช้การทำเครื่องหมายเนื้อหาและการเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)
3. ถ้าคุณต้องการเอาส่วนหัว/ส่วนท้ายที่มีอยู่ออกให้รีวิว[เอาหัวกระดาษและท้ายกระดาษออกจากโซลูชันการติดฉลากอื่นๆ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)

ถ้าคุณยังคงพบปัญหาให้รวบรวมล็อกไคลเอ็นต์การป้องกันข้อมูลของ Azure และแนบไฟล์บันทึกที่ส่งออกไปยังตั๋วนี้

**ส่งออกแฟ้มบันทึกการป้องกันข้อมูล Azure**

1. เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
2. คลิกการ**ป้องกัน/ความไว**ต่อ  >  **วิธีใช้และคำติชม**
3. คลิก**ส่งออกบันทึก**
4. บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการนี้

สำหรับข้อมูลเพิ่มเติมให้ดูที่:

- [วิธีการกำหนดค่าป้ายชื่อสำหรับเครื่องหมายภาพสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ข้อกำหนดสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [บทช่วยสอนเริ่มต้นใช้งานด่วนสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure](https://www.microsoft.com/download/details.aspx?id=53018)
