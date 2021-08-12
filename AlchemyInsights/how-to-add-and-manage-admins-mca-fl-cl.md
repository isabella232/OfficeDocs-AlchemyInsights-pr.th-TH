---
title: วิธีเพิ่มและจัดการผู้ดูแลระบบ
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
ms.openlocfilehash: 924e195740e55c53b9605a9b9bd694a72cf9951006d1dc5e888023cd6e3f9d45
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963842"
---
# <a name="how-to-add-and-manage-admins"></a>วิธีเพิ่มและจัดการผู้ดูแลระบบ

โดยยึดตามรายละเอียดปัญหาของคุณ เราพบวิธีแก้ไขปัญหาให้คุณแล้ว ลูกค้าส่วนใหญ่สามารถแก้ไขปัญหาของตนเองได้หลังจากติดตามเอกสารประกอบของเรา

เมื่อต้องการจัดการบัญชีการเรียกเก็บเงินของคุณเพื่อให้ข้อตกลงของลูกค้า Microsoft (MCA) คุณสามารถใช้บทบาทต่างๆ ที่มีระดับการเข้าถึงที่ต้องการได้ บทบาทเหล่านี้นอกเหนือจากบทบาทบริการ Azure ที่มีอยู่แล้วภายในซึ่งช่วยให้คุณควบคุมทรัพยากรของคุณ

**เมื่อต้องการเพิ่มบทบาทการเรียกเก็บเงินในพอร์ทัล Azure:**

1. ลงชื่อเข้าใช้พอร์ทัล[Azure](https://portal.azure.com/)
2. ค้นหา *การจัดการต้นทุน +* การเรียกเก็บเงิน
3. เลือก การควบคุมการเข้าถึง (IAM) ที่ขอบเขต เช่น บัญชีการเรียกเก็บเงิน โปรไฟล์การเรียกเก็บเงิน หรือส่วนใบแจ้งหนี้ที่คุณต้องการให้สิทธิ์การเข้าถึง
4. หน้า ตัวควบคุม Access (IAM) จะแสดงรายการผู้ใช้และกลุ่มที่มอบหมายให้กับแต่ละบทบาทในขอบเขตนั้น
5. เมื่อต้องการให้สิทธิ์การเข้าถึง **แก่ผู้ใช้** ให้เลือก เพิ่ม จากด้านบนของหน้า ในรายการ *ดร* อปดาวน์ บทบาท ให้เลือกบทบาท ใส่ที่อยู่อีเมลของผู้ใช้ที่คุณต้องการให้สิทธิ์การเข้าถึง **เลือก** บันทึก เพื่อกําหนดบทบาท
6. เมื่อต้องการเอาสิทธิ์การเข้าถึงของผู้ใช้ออก ให้เลือกผู้ใช้ที่มีงานที่มอบหมายบทบาทที่คุณต้องการเอาออก เลือก **เอาออก**

**เอกสารที่แนะนา**

- [นิยามบทบาทการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [บทบาทและงานของบัญชีการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [เริ่มต้นใช้งานบัญชีการเรียกเก็บเงิน MCA ของคุณ](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [ตรวจสอบการเข้าถึงข้อตกลงของลูกค้า Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
