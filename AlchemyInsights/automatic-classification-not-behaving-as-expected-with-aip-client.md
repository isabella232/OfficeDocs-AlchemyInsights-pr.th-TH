---
title: การจัดประเภทอัตโนมัติจะไม่มีลักษณะการใช้งานตามที่คาดไว้กับไคลเอ็นต์ AIP
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
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715220"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>การจัดประเภทอัตโนมัติจะไม่มีลักษณะการใช้งานตามที่คาดไว้กับไคลเอ็นต์ AIP

การจัดประเภทอัตโนมัติไม่ทำงานตามที่คาดไว้ให้ใช้แนวทางที่แนะนำต่อไปนี้:

1. ถ้าคุณกำลังมีปัญหาเกี่ยวกับการติดป้ายอัตโนมัติให้ดู[ที่วิธีกำหนดค่าเงื่อนไขสำหรับการจัดประเภทโดยอัตโนมัติและที่แนะนำสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)และ[ความต้องการของชนิดข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. ตรวจสอบว่าคุณกำลังใช้นโยบายลักษณะที่ไม่ได้รับการกำหนดค่าอย่างถูกต้อง:[วิธีการกำหนดค่านโยบายการป้องกันข้อมูล Azure สำหรับผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายลักษณะ](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. ถ้าการติดป้ายอัตโนมัติไม่ทำงานสำหรับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อให้ตรวจสอบว่า `DRMEncryptProperty` ไม่ได้กำหนดไว้ตามที่อธิบายไว้ที่นี่:[การตั้งค่ารีจิสทรี IRM สำหรับความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. ถ้าคุณใช้ [ชนิดข้อมูลที่มีอยู่แล้ว](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) สำหรับนโยบายการป้องกันข้อมูล Azure ของคุณให้ตรวจสอบว่าเนื้อหาของคุณตรงกับรูปแบบที่คาดไว้หรือไม่
5. ตรวจสอบว่ามีการกำหนดค่าป้ายชื่ออย่างเหมาะสมสำหรับ**อัตโนมัติ**หรือ**แนะนำ** (การติดฉลาก**อัตโนมัติ** พร้อมใช้งานสำหรับแอป microsoft ๓๖๕ทั้งหมดในขณะที่ **แนะนำ** จะพร้อมใช้งานสำหรับแอป microsoft ๓๖๕ทั้งหมดยกเว้น Outlook)
6. คุณไม่สามารถใช้การจัดประเภทอัตโนมัติสำหรับเอกสารและอีเมลที่มีการติดป้ายชื่อก่อนหน้านี้ด้วยตนเองหรือก่อนหน้านี้โดยอัตโนมัติที่มีการจัดประเภทที่สูงกว่า  สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การนำป้ายชื่ออัตโนมัติหรือที่แนะนำไปใช้](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. ถ้าคุณยังคงประสบปัญหาโปรดรวบรวมบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบไฟล์บันทึกที่ส่งออกไปยังตั๋วสนับสนุนของคุณ เมื่อต้องการส่งออกแฟ้มบันทึกการป้องกันข้อมูล Azure:
    - เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
    - คลิกการ**ป้องกัน/ความไว**ต่อ  >  **วิธีใช้และคำติชม**
    - คลิก**ส่งออกบันทึก**
    - บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการของคุณ

สำหรับข้อมูลเพิ่มเติมให้ดูที่:

- [วิธีการกำหนดค่าเงื่อนไขสำหรับการจัดประเภทอัตโนมัติและที่แนะนำสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [เส้นบอกแนววิธีการสำหรับสถานการณ์สมมติทั่วไปที่ใช้การป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [รีวิวการสมัครใช้งานการป้องกันข้อมูลของ Azure และฟีเจอร์](https://azure.microsoft.com/pricing/details/information-protection)
- [ข้อกำหนดสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [บทช่วยสอนเริ่มต้นใช้งานด่วนสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure](https://www.microsoft.com/download/details.aspx?id=53018)
