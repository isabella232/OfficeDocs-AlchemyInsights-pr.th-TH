---
title: เข้าถึงรีวิว
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014995"
---
# <a name="access-reviews"></a>เข้าถึงรีวิว

1. **เปิดใช้งานรีวิวการเข้าถึง**: คุณสามารถเปิดใช้งานการรีวิวเมื่อคุณสร้างแพคเกจ access ใหม่หรือแก้ไขแพคเกจการเข้าถึงที่มีอยู่ [สร้างการตรวจทานการเข้าถึงของแพคเกจการเข้าถึงในการจัดการสิทธิ์ของ AZURE AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) อธิบายวิธีการเปิดใช้งานการเข้าถึงการเข้าถึงแพคเกจ access

1. **ตรวจทานการเข้าถึง**: การจัดการสิทธิ์การใช้งาน Azure AD ช่วยลดความซับซ้อนในการจัดการการเข้าถึงกลุ่มแอปพลิเคชันและไซต์ SharePoint [ตรวจทานการเข้าถึงแพคเกจการเข้าถึงในการจัดการสิทธิ์การใช้งาน AZURE AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) อธิบายวิธีดำเนินการรีวิวการเข้าถึงสำหรับผู้ใช้อื่นที่ได้รับมอบหมายให้กับแพคเกจการเข้าถึงในฐานะผู้ตรวจทานที่ได้รับมอบหมาย

1. **ตรวจทานการเข้าถึงด้วยตัวคุณเอง**: การ [ตรวจสอบด้วยตนเองของแพคเกจการเข้าถึงในการจัดการสิทธิ์ของ AD Azure](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) อธิบายวิธีที่ผู้ใช้ตรวจทานตนเองของแพคเกจการเข้าถึงที่ได้รับมอบหมาย

1. ในกรณีส่วนใหญ่ผู้ใช้จะพบการรีวิวที่ค้างอยู่ในการตอบกลับของพวกเขาใน **แผงการเข้าถึง** การทำเช่นนี้จะสามารถใช้ได้กับความคิดเห็นของกลุ่มและแอปพลิเคชันไม่ใช่บทบาท สำหรับความคิดเห็นของ Access ทั้งหมดของบทบาทผู้ใช้จะต้องนำทางไปยังการจัดการข้อมูลประจำตัวของ Azure AD AD (PIM) เพื่อทำการตรวจทานให้เสร็จสมบูรณ์

    1. การเข้าสู่ระบบไปยังพอร์ทัล Azure
    2. นำทางไปยัง Azure AD PIM
    3. ในบานหน้าต่างนำทางด้านซ้ายให้เลือก **งาน**  >  การ **ตรวจทานการเข้าถึง**
    
สำหรับข้อมูลเพิ่มเติม ให้ดูที่

- [ดำเนินการรีวิว access ของบทบาท Azure AD Azure ของฉันใน PIM ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [ดำเนินการรีวิว access ของบทบาททรัพยากร Azure ของฉันใน PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)