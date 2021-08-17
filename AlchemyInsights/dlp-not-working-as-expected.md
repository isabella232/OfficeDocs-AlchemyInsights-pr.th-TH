---
title: DLP ไม่ใช้งานได้ตามที่คาดไว้
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
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079721"
---
# <a name="dlp-not-working-as-expected"></a>DLP ไม่ใช้งานได้ตามที่คาดไว้

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวแบบออนไลน์ SharePoint เพื่อดูข้อมูลเพิ่มเติม

 **การตั้งค่า DLP**

คุณมีปัญหากับการป้องกันการ **สูญหายของข้อมูล (DLP)** ใน Office 365ไม่เป็นไปตามที่คาดไว้หรือไม่ If so, make sure that your **DLP policy** is set up correct, and that your data contains what the **DLP policy** is looking for when it is being evaluated.
  
นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ [ข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)ต่อไปนี้
  
 **นโยบาย DLP มีลักษณะอย่างไร**
  
เมื่อใช้ชนิดข้อมูล **ที่ละเอียดอ่อนที่มีอยู่แล้วภายในศูนย์การรักษา** ความปลอดภัยและการปฏิบัติตามนโยบาย นโยบาย DLP จะค้นหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจหาชนิดที่เป็นความลับเหล่านี้
  
- **ชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**

    For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **ชนิดข้อมูลที่เป็นความลับแบบเอง**

    ถ้าคุณพยายามสร้างชนิดข้อมูลที่เป็นความลับแบบเอง ให้ใช้บทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่เป็นความลับแบบเอง: [สร้างชนิดข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)ที่เป็นความลับแบบเอง

**ทดสอบนโยบาย DLP**

เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในหรือชนิดข้อมูลที่จําเป็น ให้ใช้ **ตัวเลือก ชนิดการทดสอบ****ภายใต้ ประเภท**  >  **ข้อมูลที่ละเอียดอ่อน** For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **รายงาน**
  
- รับข้อมูลเชิงลึกด้วย [รายงาน DLP](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี [รายงาน](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)เหตุการณ์
