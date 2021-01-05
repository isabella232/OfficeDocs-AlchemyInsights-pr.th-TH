---
title: วิธีการเพิ่มและจัดการผู้ดูแลระบบ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755530"
---
# <a name="how-to-add-and-manage-admins"></a>วิธีการเพิ่มและจัดการผู้ดูแลระบบ

เราพบวิธีแก้ไขปัญหาของคุณโดยยึดตามคำอธิบายปัญหาของคุณ ลูกค้าส่วนใหญ่สามารถแก้ไขปัญหาของตนเองได้หลังจากที่ทำตามเอกสารประกอบของเราแล้ว

เมื่อต้องการจัดการบัญชีผู้ใช้สำหรับการเรียกเก็บเงินของคุณสำหรับข้อตกลงลูกค้าของ Microsoft (MCA) คุณสามารถใช้บทบาทที่แตกต่างกันกับระดับการเข้าถึงที่ต้องการได้ บทบาทเหล่านี้นอกเหนือจากบทบาทบริการ Azure ที่มีอยู่แล้วภายในซึ่งจะช่วยให้คุณสามารถควบคุมทรัพยากรของคุณได้

**เมื่อต้องการเพิ่มบทบาทการเรียกเก็บเงินในพอร์ทัล Azure ให้ใช้ดังนี้**

1. ลงชื่อเข้าใช้[พอร์ทัล Azure](https://portal.azure.com/)
2. ค้นหา *การจัดการต้นทุน + การเรียกเก็บเงิน*
3. เลือกตัวควบคุมการเข้าถึง (IAM) ที่ขอบเขตเช่นบัญชีผู้ใช้การเรียกเก็บเงินโปรไฟล์การเรียกเก็บเงินหรือใบแจ้งหนี้ที่คุณต้องการให้สิทธิ์การเข้าถึง
4. หน้า Access control (IAM) จะแสดงรายการผู้ใช้และกลุ่มที่ได้รับมอบหมายให้กับแต่ละบทบาทสำหรับขอบเขตนั้น
5. เมื่อต้องการให้สิทธิ์การเข้าถึงแก่ผู้ใช้ให้เลือก **เพิ่ม** จากด้านบนของหน้า ในรายการดรอปดาวน์ *บทบาท* ให้เลือกบทบาท ใส่ที่อยู่อีเมลของผู้ใช้ที่คุณต้องการให้สิทธิ์การเข้าถึง เลือก **บันทึก** เพื่อกำหนดบทบาท
6. เมื่อต้องการเอา access ออกจากผู้ใช้ให้เลือกผู้ใช้ที่มีการกำหนดบทบาทที่คุณต้องการเอาออก เลือก **นำออก**

**เอกสารที่แนะนำ**

- [ข้อกำหนดบทบาทของการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [บทบาทและงานของบัญชีการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [เริ่มต้นใช้งานบัญชีการเรียกเก็บเงิน MCA ของคุณ](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [ตรวจสอบการเข้าถึงข้อตกลงลูกค้าของ Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
