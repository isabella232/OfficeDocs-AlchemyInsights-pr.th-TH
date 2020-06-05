---
title: 'AIP: นโยบายไม่ทํางานตามที่คาดไว้'
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
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580784"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: นโยบายไม่ทํางานตามที่คาดไว้

การป้องกันข้อมูล azure: นโยบายไม่ทํางานตามที่คาดไว้ ให้ดูคําแนะนําต่อไปนี้สําหรับปัญหานโยบายต่าง ๆ:

1. หากคุณมีปัญหากับการทําเครื่องหมายภาพ โปรดตรวจทาน[เมื่อมีใช้เครื่องหมายภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. ถ้าคุณกําลังมีปัญหากับการติดฉลากอัตโนมัติ โปรดดู[วิธีการกําหนดค่าเงื่อนไขสําหรับการจัดประเภทอัตโนมัติและแนะนําสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)และ[ชนิดของข้อมูลที่ละเอียดอ่อนจะมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. หากคุณมีปัญหากับการป้องกันเนทีฟ / Pfile โปรดตรวจสอบ[การกําหนดค่าไฟล์ API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. ตรวจสอบว่า คุณกําลังใช้นโยบายขอบเขตที่ไม่ได้ถูกกําหนดค่าอย่างถูกต้อง:[วิธีการตั้งค่าคอนฟิกนโยบายการป้องกันข้อมูล Azure สําหรับผู้ใช้เฉพาะ โดยใช้นโยบายขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. ถ้าการติดฉลากอัตโนมัติไม่ทํางานสําหรับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่าไม่ได้กําหนด DRMEncryptProperty ตามที่อธิบายไว้ที่นี่:[การตั้งค่ารีจิสทรี IRM เพื่อความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

ถ้าคุณยังคงประสบปัญหา โปรดรวบรวมแฟ้มบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบแฟ้มบันทึกที่ส่งออกไปยังใบสั่งงานนี้

1. เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
2. คลิก**Protect/Sensitivity**  >  **วิธีใช้และคําติชม**ป้องกัน/ความไว
3. คลิก**ส่งออกแฟ้มบันทึก**
4. บันทึกบันทึกไปยังตําแหน่งที่ตั้งที่คุณเลือก และแนบไฟล์เหล่านั้นกับคําขอบริการนี้

ทรัพยากรเพิ่มเติม:

- [วิธีการกําหนดค่าป้ายชื่อสําหรับเครื่องหมายภาพสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [ตรวจทานเอกสารการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ใช้ป้ายชื่อความไวในแอป Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

