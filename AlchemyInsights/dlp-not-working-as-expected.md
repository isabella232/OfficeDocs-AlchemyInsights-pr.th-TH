---
title: DLP ไม่ทำงานตามที่คาดไว้
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679712"
---
# <a name="dlp-not-working-as-expected"></a>DLP ไม่ทำงานตามที่คาดไว้

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

 **การตั้งค่า DLP**

คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ใน Office ๓๖๕ไม่ทำงานตามที่คาดไว้ใช่หรือไม่ ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่า **นโยบาย dlp** ของคุณได้รับการตั้งค่าอย่างถูกต้องและข้อมูลของคุณมีสิ่งที่ **นโยบาย dlp** กำลังค้นหาเมื่อมีการประเมิน
  
นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่สำคัญในองค์กรของคุณได้ เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ข้อมูล[ต่อไปนี้](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **นโยบาย DLP ใดที่ค้นหา**
  
เมื่อใช้ **ชนิดข้อมูลที่มีอยู่แล้วภาย** ในในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย DLP ให้มองหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจหาชนิดที่มีความสำคัญเหล่านี้
  
- **ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายใน**

    สำหรับข้อมูลเกี่ยวกับชนิดที่มีอยู่แล้วภายในและนโยบาย DLP จะมีลักษณะอย่างไรเมื่อตรวจหาชนิดที่มีความสำคัญให้ดูที่:[ชนิดข้อมูลที่มีความสำคัญคืออะไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **ชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง**

    ถ้าคุณกำลังพยายามสร้างชนิดข้อมูลที่มีความสำคัญแบบกำหนดเองให้ใช้บทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่มีความสำคัญแบบกำหนดเอง: การ[สร้างชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**ทดสอบนโยบาย DLP**

เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในหรือแบบกำหนดเองให้ใช้ตัวเลือก**ชนิดการทดสอบ****ภายใต้การจัดประเภท**  >  **ข้อมูล**ที่มีความสำคัญ สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ทดสอบชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **รายงาน**
  
- รับข้อมูลเชิงลึกของข้อมูลที่มีความสำคัญกับ [รายงาน DLP](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
