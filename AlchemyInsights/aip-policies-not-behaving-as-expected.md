---
title: 'AIP: นโยบายไม่เป็นไปตามที่คาดไว้'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821646"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: นโยบายไม่เป็นไปตามที่คาดไว้

Azure Information Protection: นโยบายไม่เป็นไปตามที่คาดไว้ ให้ดูรายการต่อไปนี้เพื่อดูแนวทางที่แนะนําเกี่ยวกับปัญหาต่างๆ ของนโยบาย:

1. ถ้าคุณมีปัญหากับการมาร์กอัปแบบเป็นภาพ โปรดตรวจสอบ[เมื่อมีการใช้เครื่องหมายด้วยภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. ถ้าคุณมีปัญหากับการกําหนดป้ายชื่ออัตโนมัติ โปรดดู วิธีการกําหนดค่าเงื่อนไขเพื่อการจัดประเภทอัตโนมัติและแนะนาเกี่ยวกับ [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) และ ชนิดข้อมูลที่เป็นความลับ [มีลักษณะ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)อย่างไร
3. ถ้าคุณมีปัญหากับการป้องกัน Native/Pfile โปรดตรวจสอบ การกําหนด [ค่า API ของ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)ไฟล์
4. ตรวจสอบว่าคุณใช้นโยบายขอบเขตที่กําหนดค่าไม่ถูกต้องหรือไม่: วิธีกําหนดค่านโยบาย[Azure Information Protection ของผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายที่กําหนดขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. ถ้าการกําหนดป้ายชื่ออัตโนมัติไม่ใช้งานกับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่า DRMEncryptProperty ไม่ได้กําหนดไว้ตามที่อธิบายไว้ที่นี่: การตั้งค่ารีจิสทรี[IRM เพื่อความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

ถ้าคุณยังคงพบปัญหา โปรดรวบรวมบันทึกของไคลเอ็นต์ Azure Information Protection และแนบบันทึกที่ส่งออกไปยังตั๋วนี้

1. เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
2. คลิก **วิธีใช้และข้อคิดเห็นเกี่ยวกับการป้องกัน/** ระดับ  >  **ความลับ**
3. คลิก **ส่งออก** แฟ้มบันทึก
4. บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์ไปกับการร้องขอบริการนี้

แหล่งข้อมูลเพิ่มเติม:

- [วิธีการกําหนดค่าป้ายชื่อเพื่อเครื่องหมายแบบเป็นภาพเพื่อ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [ตรวจทานเอกสาร Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ใช้ป้ายชื่อระดับความลับในแอป Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

