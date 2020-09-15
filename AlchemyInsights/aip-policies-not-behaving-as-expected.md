---
title: 'AIP: นโยบายที่ไม่ถูกต้องตามที่คาดไว้'
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
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663208"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: นโยบายที่ไม่ถูกต้องตามที่คาดไว้

การป้องกันข้อมูลของ Azure: นโยบายไม่มีลักษณะการใช้งานตามที่คาดไว้ให้ดูที่คำแนะนำที่แนะนำสำหรับปัญหานโยบายต่างๆดังต่อไปนี้

1. ถ้าคุณกำลังมีปัญหาเกี่ยวกับการทำเครื่องหมายการมองเห็นโปรดตรวจทานเมื่อมีการนำการทำเครื่องหมาย[แสดงผลไปใช้](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. ถ้าคุณกำลังมีปัญหาเกี่ยวกับการติดป้ายอัตโนมัติโปรดตรวจทาน[วิธีการกำหนดค่าเงื่อนไขสำหรับการจัดประเภทโดยอัตโนมัติและที่แนะนำสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)และ[ลักษณะที่ปรากฏของชนิดข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. ถ้าคุณกำลังมีปัญหาเกี่ยวกับการป้องกันพื้นเมือง/Pfile โปรดตรวจทาน[การกำหนดค่า API ของไฟล์](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. ตรวจสอบว่าคุณกำลังใช้นโยบายลักษณะที่ไม่ได้รับการกำหนดค่าอย่างถูกต้อง:[วิธีการกำหนดค่านโยบายการป้องกันข้อมูล Azure สำหรับผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายลักษณะ](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. ถ้าการติดป้ายอัตโนมัติไม่ทำงานสำหรับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อให้ตรวจสอบว่า DRMEncryptProperty ไม่ได้ถูกกำหนดตามที่อธิบายไว้ที่นี่:[การตั้งค่ารีจิสทรี IRM สำหรับความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

ถ้าคุณยังคงพบปัญหาโปรดรวบรวมบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบไฟล์บันทึกที่ส่งออกไปยังตั๋วนี้

1. เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook
2. คลิกการ**ป้องกัน/ความไว**ต่อ  >  **วิธีใช้และคำติชม**
3. คลิก**ส่งออกบันทึก**
4. บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการนี้

แหล่งข้อมูลเพิ่มเติม:

- [วิธีการกำหนดค่าป้ายชื่อสำหรับเครื่องหมายภาพสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ใช้ป้ายความลับของแอป Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

