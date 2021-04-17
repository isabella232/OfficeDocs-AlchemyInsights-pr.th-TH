---
title: การจัดประเภทอัตโนมัติไม่เป็นไปตามที่คาดไว้กับไคลเอ็นต์ AIP
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820917"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>การจัดประเภทอัตโนมัติไม่เป็นไปตามที่คาดไว้กับไคลเอ็นต์ AIP

การจัดประเภทโดยอัตโนมัติไม่เป็นไปตามที่คาดไว้ ให้ใช้แนวทางที่แนะนําต่อไปนี้:

1. ถ้าคุณมีปัญหากับการกําหนดป้ายชื่ออัตโนมัติ ให้ดู วิธีการกําหนดค่าเงื่อนไขต่างๆ โดยอัตโนมัติและแนะนาใน [การจัดประเภท Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) และ ชนิดข้อมูลที่เป็นความลับ [มีลักษณะ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)อย่างไร
2. ตรวจสอบว่าคุณใช้นโยบายขอบเขตที่กําหนดค่าไม่ถูกต้องหรือไม่: วิธีกําหนดค่านโยบาย[Azure Information Protection ของผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายที่กําหนดขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. ถ้าการกําหนดป้ายชื่ออัตโนมัติไม่ใช้งานกับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่าไม่ได้กําหนดไว้ตามที่อธิบายไว้ `DRMEncryptProperty` ที่นี่: การตั้งค่า[รีจิสทรี IRM เพื่อความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. ถ้าคุณใช้ชนิดข้อมูลที่มีอยู่แล้ว [ภายในของนโยบาย](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) Azure Information Protection ให้ตรวจสอบว่าเนื้อหาของคุณตรงกับรูปแบบที่คาดไว้หรือไม่
5. ตรวจสอบว่าป้ายชื่อได้รับการกําหนดค่าอย่างเหมาะสมเป็น อัตโนมัติ หรือ แ **นะ****นนะ** (**การติด** ป้ายอัตโนมัติจะพร้อมใช้งานในแอป Microsoft 365 ทั้งหมด **ในขณะที่** การแนะนาจะพร้อมใช้งานในแอป Microsoft 365 ทั้งหมดยกเว้น Outlook)
6. คุณไม่สามารถใช้การจัดประเภทอัตโนมัติในเอกสารและอีเมลที่มีป้ายชื่อด้วยตนเองก่อนหน้านี้ หรือป้ายชื่อที่มีการจัดประเภทสูงกว่าโดยอัตโนมัติก่อนหน้านี้ได้  ดูข้อมูลเพิ่มเติมที่: [ป้ายชื่ออัตโนมัติหรือป้ายชื่อที่แนะนวจะถูก](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)ใช้งานอย่างไร
7. ถ้าคุณยังคงพบปัญหา โปรดรวบรวมบันทึกของไคลเอ็นต์ Azure Information Protection และแนบบันทึกที่ส่งออกไปยังตั๋วการสนับสนุนของคุณ เมื่อต้องการส่งออกบันทึก Azure Information Protection:
    - เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
    - คลิก **วิธีใช้และข้อคิดเห็นเกี่ยวกับการป้องกัน/** ระดับ  >  **ความลับ**
    - คลิก **ส่งออก** แฟ้มบันทึก
    - บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์กับการร้องขอบริการของคุณ

โปรดดูข้อมูลเพิ่มเติมที่:

- [วิธีกําหนดค่าเงื่อนไขเพื่อการจัดประเภทอัตโนมัติและแนะนวให้ใช้ใน Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [คู่มือวิธีการเกี่ยวกับสถานการณ์ทั่วไปที่ใช้ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [ตรวจทานเอกสาร Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ตรวจสอบการสมัครใช้งานและฟีเจอร์ Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [ความต้องการของ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [บทช่วยสอนเริ่มต้นใช้งานด่วนของ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [ดาวน์โหลดไคลเอ็นต์ Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
