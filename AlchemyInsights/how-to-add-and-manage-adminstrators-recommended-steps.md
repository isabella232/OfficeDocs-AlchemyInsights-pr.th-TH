---
title: วิธีการเพิ่มและจัดการผู้ดูแลระบบ - ขั้นตอนที่แนะน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339051"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>วิธีการเพิ่มและจัดการผู้ดูแลระบบ - ขั้นตอนที่แนะน

โดยยึดตามรายละเอียดปัญหาของคุณ เราพบวิธีแก้ไขปัญหาให้คุณแล้ว ลูกค้าส่วนใหญ่สามารถแก้ไขปัญหาของตนเองได้หลังจากติดตามเอกสารประกอบของเรา

**แก้ไขผู้ดูแลการสมัครใช้งานหรือผู้ดูแลระบบร่วม**

- ผู้ดูแลบัญชีสามารถแก้ไขทั้งสองบทบาทได้ ในขณะที่ผู้ดูแลระบบการสมัครใช้งานสามารถเปลี่ยนเฉพาะผู้ดูแลระบบร่วมใน [พอร์ทัล Azure](https://ms.portal.azure.com/#home)เท่านั้น
- [เพิ่มหรือเปลี่ยนผู้ดูแลระบบการสมัครใช้งาน Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**อัปเดตผู้ดูแลระบบการสมัครใช้งานหรือการสมัครใช้งาน Co-Administratorภายใน (AIRS)**

ผู้ดูแลระบบบริการหรือผู้ดูแลระบบร่วมสามารถใช้งานการแอคชันนี้ด้วยตนเองได้ โดยใช้ขั้นตอนต่อไปนี้

1. เข้าสู่ระบบพอร์ทัล [Azure แล้วคลิก](https://ms.portal.azure.com/#home)**การจัดการต้นทุน + การเรียกเก็บเงิน** ใน blade ด้านซ้าย
2. คลิกรายการสินค้าที่มีการสมัครใช้งานของคุณ การทําเช่นนี้จะเปิด ภาพรวม ของการสมัครใช้งานของคุณ
3. บน **Blade** การสมัครใช้งาน **ให้คลิก** คุณสมบัติ 
4. คลิกปุ่ม **ผู้ดูแล** บริการ
5. ใส่อีเมลของผู้ใช้ที่คุณต้องการตั้งค่าเป็นผู้ดูแลบริการ **แล้วคลิก** ตกลง

**เพิ่ม/เปลี่ยน/เอาผู้ดูแลร่วมออก**

1. เข้าสู่ระบบพอร์ทัล [Azure](https://ms.portal.azure.com/#home) ในฐานะผู้ดูแลระบบบริการ
2. [เปิด การสมัครใช้งาน](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)แล้วเลือกการสมัครใช้งาน (ผู้ดูแลร่วมสามารถมอบหมายงานที่ขอบเขตการสมัครใช้งานเท่านั้น)
3. นําทางไปยังผู้ดูแลระบบแบบคลาสสิกของ Access **(IAM)** เพิ่มผู้ดูแลระบบร่วม เพื่อเปิดบานหน้าต่าง เพิ่มผู้ดูแลระบบร่วม (ถ้าตัวเลือก เพิ่มผู้ดูแลระบบร่วม ถูกปิดใช้งาน แสดงว่าคุณไม่มีสิทธิ์  >    >    >  ) 
4. เลือกผู้ใช้ที่คุณต้องการเพิ่ม **แล้วคลิก** เพิ่ม

**ศึกษาเพิ่มเติม:**
- [เพิ่มผู้ดูแลร่วม](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [เอาผู้ดูแลร่วมออก](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [เปลี่ยนผู้ดูแลระบบบริการ](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [ดูผู้ดูแลระบบบัญชี](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [จัดการการเข้าถึงโดยใช้พอร์ทัล RBAC และ Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**เพิ่ม/ลบผู้ใช้โดยใช้ Azure Active Directory (AD)**

คุณสามารถเพิ่มผู้ใช้ใหม่หรือลบผู้ใช้ที่มีอยู่จากองค์กร Azure Active Directory (Azure AD):

1. เมื่อต้องการเพิ่มผู้ใช้ใหม่ ให้เข้าสู่ระบบพอร์ทัล [Azure](https://ms.portal.azure.com/#home) เป็นผู้ดูแลระบบผู้ใช้ขององค์กร
2. เลือก **Azure Active Directory****ผู้ใช้** เลือก ผู้ใช้ แล้วคลิก **ผู้ใช้** ใหม่
3. บนหน้า **ผู้ใช้** ให้ใส่ข้อมูลที่ต้องมี คลิกสร้าง ผู้ใช้จะถูกสร้างและเพิ่มลงในผู้เช่า Azure AD ของคุณ

**เรียนรู้เพิ่มเติม**:

- [เพิ่มผู้ใช้ใหม่](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [ลบผู้ใช้](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [เพิ่มหรืออัปเดตข้อมูลโปรไฟล์ของผู้ใช้Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**เอกสารที่แนะนา**

- [การควบคุมการเข้าถึงตามบทบาท (RBAC) คืออะไร](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [เข้าใจบทบาทต่างๆ ใน Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [สิทธิ์ของบทบาทผู้ดูแลระบบใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [บทช่วยสอน: ให้สิทธิ์การเข้าถึงแก่ผู้ใช้โดยใช้ RBAC และพอร์ทัล Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [แก้ไขปัญหา RBAC ใน Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [จัดระเบียบแหล่งข้อมูลของคุณด้วยกลุ่มการจัดการ Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [วิธีการขอรับสําเนาของใบแจ้งหนี้ Azure ทางอีเมล](https://azure.microsoft.com/blog/azure-email-invoices/)
- [วิธีเพิ่ม อัปเดต หรือลบบัตรเครดิตหรือบัตรเดบิตออกจาก Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [จัดการ (เปิดใช้งานการสมัครใช้งานใหม่/ยกเลิก/สลับ)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



