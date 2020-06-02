---
title: 'AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: 418362beea221a7cb9d8fd4be6cfc0f28022093d
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493409"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้

ถ้าคุณประสบปัญหาเกี่ยวกับการทําเครื่องหมายภาพไม่แสดงตามที่คาดไว้ ให้ดูแนวทางต่อไปนี้:

1. ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน[เมื่อมีการใช้เครื่องหมายภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. สําหรับการติดฉลาก Office ให้ตรวจทาน[เมื่อ Office 365 ใช้การทําเครื่องหมายเนื้อหาและการเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)
3. ถ้าคุณต้องการเอาหัวกระดาษ/ท้ายกระดาษที่มีอยู่ออก ให้[ตรวจทาน เอาหัวกระดาษและท้ายกระดาษออกจากโซลูชันการติดฉลากอื่นๆ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)

ถ้าคุณยังคงประสบปัญหา ให้เก็บรวบรวมแฟ้มบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบแฟ้มบันทึกที่ส่งออกไปยังใบสั่งงานนี้

**ส่งออกแฟ้มบันทึกการป้องกันข้อมูล Azure**

1. เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
2. คลิก**Protect/Sensitivity**  >  **วิธีใช้และคําติชม**ป้องกัน/ความไว
3. คลิก**ส่งออกแฟ้มบันทึก**
4. บันทึกบันทึกไปยังตําแหน่งที่ตั้งที่คุณเลือก และแนบไฟล์เหล่านั้นกับคําขอบริการนี้

สําหรับข้อมูลเพิ่มเติม โปรดดู:

- [วิธีการกําหนดค่าป้ายชื่อสําหรับเครื่องหมายภาพสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [ตรวจทานเอกสารการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ข้อกําหนดสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [บทช่วยสอนเริ่มต้นใช้งานอย่างย่อสําหรับการปกป้องข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure](https://www.microsoft.com/download/details.aspx?id=53018)
