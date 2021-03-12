---
title: DLP ไม่ใช้งานตามที่คาดไว้
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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707829"
---
# <a name="dlp-not-working-as-expected"></a>DLP ไม่ใช้งานตามที่คาดไว้

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติการเป็นประวัติการเหล่านี้ เราอยู่ในระหว่างขั้นตอนเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่โปรดเยี่ยมชมการปรับปรุงฟีเจอร์ชั่วคราวของ [SharePoint Online](https://aka.ms/ODSPAdjustments) เพื่อดูข้อมูลเพิ่มเติม

 **การตั้งค่า DLP**

คุณมีปัญหากับการป้องกันการ **สูญหายของข้อมูล (DLP)** ใน Office 365 ไม่เป็นไปตามที่คาดไว้หรือไม่ If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.
  
นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ [ข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)ที่นี่
  
 **นโยบาย DLP มีลักษณะอย่างไร**
  
เมื่อใช้ชนิดข้อมูล **ที่ละเอียดอ่อนที่มีอยู่แล้วภายในใน** ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย นโยบาย DLP จะค้นหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจหาชนิดที่เป็นความลับเหล่านี้
  
- **ชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**

    For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **ชนิดข้อมูลที่เป็นความลับแบบเอง**

    ถ้าคุณพยายามสร้างชนิดข้อมูลที่มีความอ่อนไหวแบบเอง ให้ใช้บทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่เป็นความลับที่แบบปรับแต่งเอง:[สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**ทดสอบนโยบาย DLP**

เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในหรือแบบจําเป็น ให้ใช้ตัวเลือก **ชนิดการทดสอบ****ภายใต้ชนิดข้อมูล**  >  **ที่ละเอียดอ่อนของ** การจัดประเภท For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **รายงาน**
  
- รับข้อมูลเชิงลึกด้วย [รายงาน DLP](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
