---
title: การตรวจสอบการเข้าถึงตามเงื่อนไข
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708693"
---
# <a name="monitoring-conditional-access-for-exchange"></a>การตรวจสอบการเข้าถึงตามเงื่อนไขใน Exchange

ผู้ใช้ที่เป็นเป้าหมายของการเข้าถึงตามเงื่อนไขจะได้รับอีเมลแจ้งเตือนถ้าพวกเขาไม่ตรงตามข้อกฎหมายการเข้าถึงขององค์กรของคุณ เมื่อต้องการแก้ไขปัญหา เราขอแนะนนะให้แก้ไขปัญหาอย่างน้อยหนึ่งวิธีต่อไปนี้:

- ถ้าอุปกรณ์ได้รับการลงทะเบียนแล้ว ให้แนะนาให้ผู้ใช้ไปที่แอป Company Portal และตรวจสอบว่าอุปกรณ์ปรากฏในพอร์ทัลของบริษัท ถ้าไม่ ผู้ใช้ควรลงทะเบียนอุปกรณ์
- ในพอร์ทัล Azure ให้ไปที่ Intuned >ปฏิบัติตามนโยบายอุปกรณ์ ภายใต้ ตรวจสอบ ให้คลิก การปฏิบัติตามนโยบายอุปกรณ์ ดูรายงานการปฏิบัติตามนโยบายของอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้มีเครื่องหมายเป็นปฏิบัติตามนโยบายแล้ว
- ในพอร์ทัล Azure ให้ไปที่ Intuned >ปฏิบัติตามนโยบายอุปกรณ์ ภายใต้ จัดการ ให้คลิก นโยบาย ในรายการนโยบายการปฏิบัติตามนโยบาย ให้ตรวจสอบว่าโปรไฟล์ถูกมอบหมายให้กับอุปกรณ์ของผู้ใช้ของคุณ ถ้าไม่มีการมอบหมายโปรไฟล์ Intun1 จะไม่สามารถยืนยันสถานะการปฏิบัติตามนโยบายของอุปกรณ์ได้
- แก้ไขการมอบหมายการเข้าถึงตามเงื่อนไขของผู้ใช้

1. ในพอร์ทัล Azure ให้ไปที่ **นโยบายการเข้าถึงตามเงื่อนไขของ Intuned**  >    >  
2. เลือกนโยบายจากรายการ
3. คลิก ผู้ใช้และกลุ่ม
4. เมื่อต้องการตั้งเป้าหมายนโยบายใดนโยบายหนึ่งให้กับบางคน ให้เพิ่มพวกเขาลงในรายการ รวม เพื่อให้แน่ใจว่าได้ละเว้นบุคคลใดบุคคลหนึ่งจากนโยบาย ให้เพิ่มบุคคลนั้นลงในรายการ ยกเว้น

ลิงก์ที่เป็นประโยชน์:

[ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)

[การแก้ไขปัญหา CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[การแก้ไขปัญหานโยบาย](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[การตรวจสอบการปฏิบัติตามนโยบายอุปกรณ์ Intun1](https://docs.microsoft.com/intune/compliance-policy-monitor)

หมายเหตุ: ขั้นตอนเหล่านี้มีประโยชน์ในการแก้ไขปัญหาการเข้าถึงตามเงื่อนไขของฟีเจอร์ Azure Active Directory เท่านั้น นอกจากนี้ยังสามารถกักกันอุปกรณ์ที่บล็อกการเข้าถึงอีเมลด้วยนโยบาย Exchange ข้อมูลเพิ่มเติมเกี่ยวกับการจัดการอุปกรณ์ Exchange สามารถพบได้ [ที่นี่ https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) ](
