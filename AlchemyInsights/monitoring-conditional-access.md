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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975120"
---
# <a name="monitoring-conditional-access-for-exchange"></a>การตรวจสอบการเข้าถึงตามเงื่อนไขExchange

ผู้ใช้ที่เป็นเป้าหมายของการเข้าถึงตามเงื่อนไขจะได้รับอีเมลแจ้งเตือนถ้าพวกเขาไม่ผ่านข้อต้องการเข้าถึงขององค์กรของคุณ เมื่อต้องการแก้ไขปัญหา เราขอแนะนนะให้โซลูชันอย่างน้อยหนึ่งวิธีต่อไปนี้:

- ถ้าอุปกรณ์นี้ได้รับการยืนยันว่าได้รับการลงทะเบียนแล้ว ให้แนะCompany Portalให้ผู้ใช้ไปที่แอป Company Portal ถ้าไม่ ผู้ใช้ควรลงทะเบียนอุปกรณ์
- ในพอร์ทัล Azure ให้ไปที่ Intun>การปฏิบัติตามนโยบายอุปกรณ์ ภายใต้ จอภาพ ให้คลิก การปฏิบัติตามนโยบายอุปกรณ์ ดูรายงานการปฏิบัติตามนโยบายอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้มีเครื่องหมายเป็นปฏิบัติตามนโยบายแล้ว
- ในพอร์ทัล Azure ให้ไปที่ Intun>การปฏิบัติตามนโยบายอุปกรณ์ ภายใต้ จัดการ ให้คลิก นโยบาย ในรายการนโยบายการปฏิบัติตามนโยบาย ให้ตรวจสอบว่าโปรไฟล์ถูกมอบหมายให้กับอุปกรณ์ของผู้ใช้ของคุณ ถ้าไม่มีการมอบหมายโปรไฟล์ Intuny จะไม่สามารถยืนยันสถานะการปฏิบัติตามนโยบายของอุปกรณ์ได้
- แก้ไขการมอบหมายการเข้าถึงตามเงื่อนไขของผู้ใช้

1. ในพอร์ทัล Azure ให้ไปที่ **นโยบายการเข้าถึงตามเงื่อนไขของ Intuned**  >    >  
2. เลือกนโยบายจากรายการ
3. คลิก ผู้ใช้และกลุ่ม
4. เมื่อต้องการตั้งเป้าหมายนโยบายใดนโยบายหนึ่งให้กับบางคน ให้เพิ่มพวกเขาลงในรายการ รวม เพื่อให้แน่ใจว่าได้ละเว้นบุคคลจากนโยบายให้เพิ่มบุคคลดังกล่าวลงในรายการ ยกเว้น

ลิงก์ที่มีประโยชน์:

[ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)

[การแก้ไขปัญหา CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[การแก้ไขปัญหานโยบาย](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[การตรวจสอบการปฏิบัติตามนโยบายอุปกรณ์ Intun1](https://docs.microsoft.com/intune/compliance-policy-monitor)

หมายเหตุ: ขั้นตอนเหล่านี้มีประโยชน์ในการแก้ไขปัญหาฟีเจอร์Azure Active Directoryการเข้าถึงตามเงื่อนไขเท่านั้น นอกจากนี้ยังสามารถกักกันอุปกรณ์ที่บล็อกการเข้าถึงอีเมลด้วยExchangeของคุณ ข้อมูลเพิ่มเติมเกี่ยวกับExchangeการจัดการอุปกรณ์สามารถพบได้ [ที่นี่ https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) ](
