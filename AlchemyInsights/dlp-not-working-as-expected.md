---
title: DLP ไม่ทํางานตามที่คาดไว้
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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977457"
---
# <a name="dlp-not-working-as-expected"></a>DLP ไม่ทํางานตามที่คาดไว้

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

 **การตั้งค่า DLP**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ใน Office 365 ไม่ทํางานตามที่คาดไว้หรือไม่ ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง และว่า ข้อมูลของคุณประกอบด้วย**นโยบาย DLP**กําลังค้นหาเมื่อมีการประเมิน
  
นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ข้อมูล[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **สิ่งที่นโยบาย DLP มองหา**
  
เมื่อใช้**ชนิดข้อมูลที่สําคัญที่มีอยู่แล้วภายใน**ใน Office 365 Security and Compliance Center นโยบาย DLP จะค้นหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจพบชนิดที่ละเอียดอ่อนเหล่านี้
  
- **ชนิดข้อมูลที่ละเอียดอ่อนในตัว**

    สําหรับข้อมูลเกี่ยวกับชนิดที่ละเอียดอ่อนที่มีอยู่แล้วภายใน และนโยบาย DLP จะค้นหาอะไรเมื่อตรวจหาชนิดอ่อนไหว ให้ดูที่:[ชนิดของข้อมูลที่ละเอียดอ่อนจะค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- **ชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**

    ถ้าคุณกําลังพยายามสร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง ให้ใช้บทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่ละเอียดอ่อนแบบกําหนดเอง:[สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)

**ทดสอบนโยบาย DLP**

เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่ละเอียดอ่อนในตัวหรือแบบกําหนดเอง ให้ใช้ตัวเลือก**ประเภทการทดสอบ**ภายใต้**Classifications** > **ชนิดข้อมูลที่ละเอียดอ่อน** สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ทดสอบชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)

 **รายงาน**
  
- รับข้อมูลเชิงลึกของข้อมูลที่ละเอียดอ่อนด้วย[รายงาน DLP](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)
