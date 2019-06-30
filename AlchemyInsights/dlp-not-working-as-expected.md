---
title: DLP ไม่ทำงานตามที่คาดไว้
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 3d8316502b4e51a101197a908cf691f0ab7f845a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389632"
---
# <a name="dlp-not-working-as-expected"></a>DLP ไม่ทำงานตามที่คาดไว้

คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ใน Office 365 ไม่ทำงานตามที่คาดไว้หรือไม่ ถ้าเป็นเช่นนั้น ให้แน่ใจ ว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง ว่า ข้อมูลของคุณประกอบด้วยอะไร**นโยบาย DLP**จะค้นหาเมื่อมีการประเมิน
  
 **การตั้งค่า DLP:**
  
นโยบาย DLP ช่วยให้คุณสามารถระบุ และปกป้องข้อมูลที่สำคัญในองค์กรของคุณ เมื่อต้องการตั้งค่านโยบาย DLP ใช้รายละเอียด[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **นโยบาย DLP สิ่งที่ค้นหา:**
  
เมื่อใช้**ชนิดของข้อมูลที่สำคัญที่มีอยู่แล้วภาย**ใน Office 365 ปลอดภัยและปฏิบัติตามกฎระเบียบศูนย์ นโยบาย DLP ค้นหาเฉพาะรูปแบบและองค์ประกอบเมื่อตรวจพบชนิดเหล่านี้เป็นความลับ
  
- **ชนิดของข้อมูลที่สำคัญอยู่แล้วภายใน:**

    สำหรับข้อมูลเกี่ยวกับชนิดสำคัญมีอยู่ภายในและอะไรนโยบาย DLP ค้นหาเมื่อทำการตรวจหาชนิดใบสำคัญ ดู:[ชนิดข้อมูลที่เป็นความลับค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- **ชนิดข้อมูลแบบกำหนดเองที่สำคัญ:**

    ถ้าคุณกำลังพยายามสร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ ใช้บทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดสำคัญแบบกำหนดเอง:[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)

 **รายงาน:**
  
- รับความเข้าใจข้อมูลที่สำคัญด้วย[DLP รายงาน](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- ดูรายละเอียดเฉพาะของเหตุการณ์ที่มีการ[รายงานเหตุการณ์](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)
