---
title: DLP ไม่ทํางานตามที่คาดไว้
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507497"
---
# <a name="dlp-not-working-as-expected"></a>DLP ไม่ทํางานตามที่คาดไว้

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

 **การตั้งค่า DLP**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ใน Office 365 ไม่ทํางานตามที่คาดไว้หรือไม่ ตรวจสอบให้แน่ใจว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง และว่าข้อมูลของคุณประกอบด้วยสิ่งที่**นโยบาย DLP**กําลังค้นหาเมื่อมีการประเมิน
  
นโยบาย DLP ช่วยให้คุณสามารถระบุและป้องกันข้อมูลที่ละเอียดอ่อนในองค์กรของคุณ เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ข้อมูล[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **นโยบาย DLP มองหาอะไร**
  
เมื่อใช้**ชนิดข้อมูลที่ละเอียดอ่อนในตัว**ในศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบนโยบาย DLP จะค้นหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจพบชนิดที่สําคัญเหล่านี้
  
- **ประเภทข้อมูลที่ละเอียดอ่อนในตัว**

    สําหรับข้อมูลเกี่ยวกับชนิด Sensitive ที่มีอยู่แล้วภายใน และนโยบาย DLP จะค้นหาเมื่อตรวจพบชนิด Sensitive ให้ดูที่:[ชนิดของข้อมูลที่ละเอียดอ่อนจะมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **ประเภทข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**

    ถ้าคุณกําลังพยายามสร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง ให้ใช้บทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่สําคัญแบบกําหนดเอง:[สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**ทดสอบนโยบาย DLP**

เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่มีความไวในตัวหรือแบบกําหนดเอง ให้ใช้ตัวเลือก**ประเภทการทดสอบ**ภายใต้**Classifications**  >  **ประเภทข้อมูลละเอียดอ่อน**ของการจําแนกประเภท สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การทดสอบชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **รายงาน**
  
- รับข้อมูลเชิงลึกที่ละเอียดอ่อนด้วย[รายงาน DLP](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
