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
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934312"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: นโยบายไม่เป็นไปตามที่คาดไว้

Azure Information Protection: นโยบายไม่เป็นไปตามที่คาดไว้ ให้ดูรายการต่อไปนี้เพื่อดูแนวทางที่แนะนําเกี่ยวกับปัญหาต่างๆ ของนโยบาย:

1. ถ้าคุณมีปัญหากับการมาร์กอัปแบบเป็นภาพ โปรดตรวจสอบ[เมื่อมีการใช้เครื่องหมายด้วยภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. ถ้าคุณมีปัญหากับการกําหนดป้ายชื่ออัตโนมัติ โปรดดู วิธีการกําหนดค่าเงื่อนไขเพื่อการจัดประเภทอัตโนมัติและแนะนาเกี่ยวกับ [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) และ ชนิดข้อมูลที่เป็นความลับ [มีลักษณะ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)อย่างไร
3. ถ้าคุณมีปัญหากับการป้องกัน Native/Pfile โปรดตรวจสอบ การกําหนด [ค่า API ของ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)ไฟล์
4. ตรวจสอบว่าคุณใช้นโยบายขอบเขตที่กําหนดค่าไม่ถูกต้องหรือไม่: วิธีกําหนดค่านโยบาย[Azure Information Protection ของผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายที่กําหนดขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. ถ้าการกําหนดป้ายชื่ออัตโนมัติไม่Outlookเมื่อคุณแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่า DRMEncryptProperty ไม่ได้กําหนดไว้ตามที่อธิบายไว้ที่นี่: การตั้งค่ารีจิสทรี[IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)เพื่อความปลอดภัย

ถ้าคุณยังคงพบปัญหา โปรดรวบรวมบันทึกของไคลเอ็นต์ Azure Information Protection และแนบบันทึกที่ส่งออกไปยังตั๋วนี้

1. เปิดOfficeเอกสารหรือสร้างอีเมลใหม่ในOutlookใหม่
2. คลิก **วิธีใช้และข้อคิดเห็นเกี่ยวกับการป้องกัน/** ระดับ  >  **ความลับ**
3. คลิก **ส่งออก** แฟ้มบันทึก
4. บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์ไปกับการร้องขอบริการนี้

แหล่งข้อมูลเพิ่มเติม:

- [วิธีการกําหนดค่าป้ายชื่อเพื่อเครื่องหมายแบบเป็นภาพเพื่อ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [ตรวจทานเอกสาร Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ใช้ป้ายชื่อระดับความลับในMicrosoft 365แอปของคุณ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

