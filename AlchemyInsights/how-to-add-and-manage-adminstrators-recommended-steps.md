---
title: วิธีการเพิ่มและจัดการ adminstrators-ขั้นตอนที่แนะนำ
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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678869"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>วิธีการเพิ่มและจัดการ adminstrators-ขั้นตอนที่แนะนำ

**แก้ไขผู้ดูแลระบบการสมัครใช้งานหรือผู้ดูแลระบบร่วม**

- ผู้ดูแลระบบบัญชีผู้ใช้สามารถแก้ไขทั้งสองบทบาทได้ในขณะที่ผู้ดูแลระบบการสมัครใช้งานสามารถเปลี่ยนได้เฉพาะผู้ดูแลร่วมใน [พอร์ทัล Azure](https://ms.portal.azure.com/#home)เท่านั้น
- [เพิ่มหรือเปลี่ยนแปลงผู้ดูแลการสมัครใช้งาน Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**อัปเดตผู้ดูแลการสมัครใช้งานหรือการสมัครใช้งาน Co-Administrator สำหรับการสมัครใช้งานภายใน (ออก)**

ผู้ดูแลระบบบริการหรือผู้ดูแลร่วมสามารถใช้งานการกระทำนี้ได้โดยใช้ขั้นตอนต่อไปนี้:

1. ลงชื่อเข้าใช้ใน [พอร์ทัล Azure](https://ms.portal.azure.com/#home) แล้วคลิก **การจัดการต้นทุน + การเรียกเก็บเงิน** ในใบมีดซ้าย
2. คลิกบรรทัดรายการที่มีการสมัครใช้งานของคุณ ซึ่งจะเป็นการเปิดภาพรวมสำหรับการสมัครใช้งานของคุณ
3. บนใบมีดการ **สมัคร** ใช้งานให้คลิก **คุณสมบัติ** 
4. คลิกปุ่ม **ผู้ดูแลระบบบริการ**
5. ใส่อีเมลของผู้ใช้ที่คุณต้องการตั้งค่าเป็นผู้ดูแลระบบบริการแล้วคลิก **ตกลง**

**เพิ่ม/เปลี่ยน/เอาผู้ดูแลร่วมออก**

1. ลงชื่อเข้าใช้ [พอร์ทัล Azure](https://ms.portal.azure.com/#home) ในฐานะผู้ดูแลระบบบริการ
2. เปิดการ [สมัคร](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ใช้งานแล้วเลือกการสมัครใช้งาน (Adminstrators สามารถกำหนดได้เฉพาะในขอบเขตการสมัครใช้งานเท่านั้น)
3. นำทางไปยังผู้ดูแลการ **เข้าถึงตัวควบคุม (IAM)**  >  **Classic**  >  **เพิ่ม**  >  **เพิ่มผู้ดูแล** เมื่อต้องการเปิดบานหน้าต่าง **เพิ่มการจัดการร่วม**(ถ้ามีการปิดใช้งานตัวเลือกเพิ่มการดูแลระบบ) แสดงว่าคุณไม่มีสิทธิ์)
4. เลือกผู้ใช้ที่คุณต้องการเพิ่มแล้วคลิก **เพิ่ม**

**ศึกษาเพิ่มเติม:**
- [เพิ่มผู้ดูแลร่วม](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [เอาผู้ดูแลร่วมออก](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [เปลี่ยนผู้ดูแลระบบบริการ](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [ดูผู้ดูแลระบบบัญชีผู้ใช้](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [จัดการการเข้าถึงโดยใช้ RBAC และพอร์ทัล Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**เพิ่ม/ลบผู้ใช้ที่ใช้ Azure Active Directory (AD)**

คุณสามารถเพิ่มผู้ใช้ใหม่หรือลบผู้ใช้ที่มีอยู่ออกจากองค์กร Azure Active Directory (Azure AD) ของคุณได้ดังนี้

1. เมื่อต้องการเพิ่มผู้ใช้ใหม่ให้เข้าสู่ระบบ [พอร์ทัล Azure](https://ms.portal.azure.com/#home) เป็นผู้ดูแลระบบผู้ใช้สำหรับองค์กร
2. เลือก **Azure Active directory** เลือก **ผู้ใช้** แล้วคลิก **ผู้ใช้ใหม่**
3. บนหน้า **ผู้ใช้** ให้กรอกข้อมูลที่จำเป็น คลิก **สร้าง** ผู้ใช้จะถูกสร้างขึ้นและเพิ่มลงในผู้เช่า Azure AD ของคุณ

**เรียนรู้เพิ่มเติม**:

- [เพิ่มผู้ใช้ใหม่](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [ลบผู้ใช้](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [เพิ่มหรืออัปเดตข้อมูลโปรไฟล์ของผู้ใช้โดยใช้ Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**เอกสารที่แนะนำ**

- [การควบคุมการเข้าถึงตามบทบาท (RBAC) คืออะไร](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [ทำความเข้าใจบทบาทที่แตกต่างกันใน Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [สิทธิ์ของบทบาทผู้ดูแลระบบใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [บทช่วยสอน: ให้สิทธิ์การเข้าถึงสำหรับผู้ใช้ที่ใช้ RBAC และพอร์ทัล Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [แก้ไขปัญหา RBAC ใน Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [จัดระเบียบทรัพยากรของคุณด้วยกลุ่มการจัดการ Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [วิธีการร้องขอสำเนาใบแจ้งหนี้ของ Azure ผ่านทางอีเมล](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [วิธีการเพิ่มอัปเดตหรือเอาบัตรเครดิตหรือบัตรเดบิตออกจาก Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [การสมัครใช้งาน (เปิดใช้งาน/ยกเลิก/สลับ)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



