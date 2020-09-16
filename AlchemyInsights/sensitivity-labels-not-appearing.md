---
title: ป้ายชื่อความลับไม่ปรากฏขึ้น
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801203"
---
# <a name="sensitivity-labels-not-appearing"></a>ป้ายชื่อความลับไม่ปรากฏขึ้น

ป้ายความลับจะช่วยให้คุณสามารถจัดประเภทและช่วยป้องกันเนื้อหาที่มีความสำคัญของคุณได้ พวกเขาสามารถสร้างขึ้นได้ในศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕, ศูนย์การรักษาความปลอดภัยของ microsoft ๓๖๕หรือ Microsoft ๓๖๕ความปลอดภัย & ศูนย์การปฏิบัติตามนโยบายภายใต้การจัดประเภท > ป้ายชื่อความลับ เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับฟีเจอร์นี้ให้ดู[ที่ภาพรวมของป้ายชื่อความลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

ถ้าคุณกำหนดค่าป้ายชื่อความลับของคุณแต่ไม่ปรากฏในแอป Microsoft ๓๖๕ให้ตรวจสอบสิ่งต่อไปนี้:

- ยืนยันว่ามีการ [เผยแพร่](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) ป้ายความลับของผู้ใช้และกลุ่มที่คุณต้องการ

- ยืนยันว่าผู้ใช้กำลังใช้แอปที่สนับสนุนป้ายชื่อความลับ-ดู[ป้ายชื่อความลับในเอกสารของคุณ](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- ถ้าคุณกำลัง[โยกย้ายป้ายชื่อการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)โปรดทราบข้อควรพิจารณาที่แสดงรายการไว้[ที่นี่](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- การสนับสนุนการป้องกันการสูญหายของข้อมูล (DLP): ในขณะนี้มีเฉพาะป้ายการเก็บข้อมูลเท่านั้นที่สามารถใช้เป็นเงื่อนไขในนโยบาย DLP ได้  การสนับสนุนสำหรับป้ายชื่อความลับในนโยบาย DLP ยังไม่พร้อมใช้งานแต่เรากำลังทำงานอยู่

- เมื่อมีการเปิดใช้งานการเข้ารหัสลับบนป้ายชื่อความลับคุณสามารถเลือกได้ว่าจะ:
    - กำหนดสิทธิ์เดี๋ยวนี้
    - อนุญาตให้ผู้ใช้กำหนดสิทธิ์


สำหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาที่เป็นไปได้ให้ดู[ที่ปัญหาที่ทราบเกี่ยวกับป้ายชื่อความลับ](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)