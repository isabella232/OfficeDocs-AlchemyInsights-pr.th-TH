---
title: ป้ายชื่อระดับความลับไม่ปรากฏขึ้น
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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061451"
---
# <a name="sensitivity-labels-not-appearing"></a>ป้ายชื่อระดับความลับไม่ปรากฏขึ้น

ป้ายชื่อระดับความลับช่วยให้คุณสามารถจัดประเภทและช่วยปกป้องเนื้อหาที่ละเอียดอ่อนของคุณ ซึ่งสามารถสร้างขึ้นในศูนย์การรักษาความปลอดภัยของ ศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 Microsoft 365หรือศูนย์การรักษาMicrosoft 365มาตรฐาน&ภายใต้การจัดประเภทและ>ระดับความลับ เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับฟีเจอร์นี้ ให้ดู [ภาพรวมของป้ายชื่อระดับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)ความลับ

ถ้าคุณกําหนดค่าป้ายชื่อระดับความลับของคุณแต่ไม่ปรากฏในMicrosoft 365แอป ให้ตรวจสอบดังต่อไปนี้:

- ยืนยันว่าป้ายระดับความลับได้รับการ [เผยแพร่](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) ไปยังผู้ใช้และกลุ่มที่คุณต้องการแล้ว

- ยืนยันว่าผู้ใช้ใช้แอปที่สนับสนุนป้ายชื่อระดับความลับ - ดู [ป้ายชื่อระดับความลับในเอกสาร](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)ของคุณ

- หากคุณจะ [โยกย้ายป้ายชื่อ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)ให้ระวังข้อควรพิจารณา [ที่ระบุไว้](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)ที่นี่

- การสนับสนุนการป้องกันการสูญหายของข้อมูล (DLP) : ในปัจจุบัน มีเพียงป้ายชื่อการเก็บข้อมูลเท่านั้นที่สามารถใช้เป็นเงื่อนไขในนโยบาย DLP ได้  การสนับสนุนป้ายระดับความลับในนโยบาย DLP ยังไม่พร้อมใช้งาน แต่เรายังคงแก้ไขอยู่

- เมื่อเปิดใช้งานการเข้ารหัสลับบนป้ายระดับความลับ คุณสามารถเลือกอย่างใดอย่างหนึ่งต่อไปนี้
    - กําหนดสิทธิ์ทันที
    - อนุญาตให้ผู้ใช้กําหนดสิทธิ์


For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).