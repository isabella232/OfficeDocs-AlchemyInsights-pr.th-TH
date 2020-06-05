---
title: การจัดประเภทอัตโนมัติไม่ทําตามที่คาดไว้กับไคลเอนต์ AIP
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
- "4373"
ms.openlocfilehash: 8c79ab50e7ddbda0cf61eb9a95279f6c42cc515c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581214"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>การจัดประเภทอัตโนมัติไม่ทําตามที่คาดไว้กับไคลเอนต์ AIP

การจัดประเภทอัตโนมัติไม่ปฏิบัติตามที่คาดไว้ให้ใช้แนวทางที่แนะนําต่อไปนี้:

1. ถ้าคุณมีปัญหากับการติดฉลากอัตโนมัติ ให้ดูที่[วิธีกําหนดค่าเงื่อนไขสําหรับการจัดประเภทอัตโนมัติและแนะนําสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)และ[ชนิดของข้อมูลที่ละเอียดอ่อนจะมีลักษณะ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)อย่างไร
2. ตรวจสอบว่า คุณกําลังใช้นโยบายขอบเขตที่ไม่ได้ถูกกําหนดค่าอย่างถูกต้อง:[วิธีการตั้งค่าคอนฟิกนโยบายการป้องกันข้อมูล Azure สําหรับผู้ใช้เฉพาะ โดยใช้นโยบายขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. ถ้าการติดฉลากอัตโนมัติไม่ทํางานสําหรับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่า `DRMEncryptProperty` ไม่ได้กําหนดเป็นอธิบายไว้ที่นี่:[การตั้งค่ารีจิสทรี IRM สําหรับการรักษาความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. ถ้าคุณใช้[ชนิดข้อมูลที่มีอยู่แล้วภายใน](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)สําหรับนโยบายการป้องกันข้อมูล Azure ของคุณ ให้ตรวจสอบว่าเนื้อหาของคุณตรงกับรูปแบบที่คาดไว้หรือไม่
5. ตรวจสอบว่ามีการกําหนดค่าป้ายชื่ออย่างเหมาะสมสําหรับ**อัตโนมัติ**หรือ**แนะนํา** (การติดฉลาก**อัตโนมัติ**จะพร้อมใช้งานสําหรับแอป Microsoft 365 ทั้งหมด ในขณะที่**แนะนํา**จะพร้อมใช้งานสําหรับแอป Microsoft 365 ทั้งหมด ยกเว้น Outlook)
6. คุณไม่สามารถใช้การจัดประเภทอัตโนมัติสําหรับเอกสารและอีเมลที่ก่อนหน้านี้ด้วยตนเองหรือก่อนหน้านี้มีป้ายชื่อโดยอัตโนมัติด้วยการจัดประเภทที่สูงขึ้น  สําหรับข้อมูลเพิ่มเติม ให้ดูที่:[วิธีนําป้ายชื่ออัตโนมัติหรือที่แนะนําไปใช้](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. ถ้าคุณยังคงประสบปัญหา โปรดรวบรวมแฟ้มบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบแฟ้มบันทึกที่ส่งออกไปยังตั๋วสนับสนุนของคุณ เมื่อต้องการส่งออกแฟ้มบันทึกการป้องกันข้อมูล Azure:
    - เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
    - คลิก**Protect/Sensitivity**  >  **วิธีใช้และคําติชม**ป้องกัน/ความไว
    - คลิก**ส่งออกแฟ้มบันทึก**
    - บันทึกบันทึกไปยังตําแหน่งที่ตั้งที่คุณเลือก และแนบไฟล์เหล่านั้นกับคําขอบริการของคุณ

สําหรับข้อมูลเพิ่มเติม โปรดดู:

- [วิธีการกําหนดค่าเงื่อนไขสําหรับการจัดประเภทอัตโนมัติและแนะนําสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [คําแนะนําวิธีการสําหรับสถานการณ์สมมติทั่วไปที่ใช้การป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [ตรวจทานเอกสารการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ตรวจทานการสมัครใช้งานและคุณลักษณะการป้องกันข้อมูลของ Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [ข้อกําหนดสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [บทช่วยสอนเริ่มต้นใช้งานอย่างย่อสําหรับการปกป้องข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure](https://www.microsoft.com/download/details.aspx?id=53018)
