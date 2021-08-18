---
title: อัปเดตที่อยู่ที่ขายให้กับและใบเรียกเก็บเงินที่เชื่อมโยงกับ MCA ของคุณ - ขั้นตอนที่แนะนา
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 5c0f4e7e92081a60be1f6930100ed08ce91ad545
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320049"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a>อัปเดตที่อยู่ที่ขายให้กับและใบเรียกเก็บเงินที่เชื่อมโยงกับ MCA ของคุณ - ขั้นตอนที่แนะนา

คุณสามารถอัปเดตที่อยู่ของขายให้กับและใบเรียกเก็บเงินที่เชื่อมโยงกับข้อตกลงของลูกค้า Microsoft (MCA) ของคุณ 

**หมายเหตุ**: เฉพาะผู้ดูแลระบบผู้ใช้เท่านั้นที่สามารถเปลี่ยนแปลงข้อมูลAzure Active Directoryโปรไฟล์ผู้ใช้ได้ ถ้าคุณไม่ได้ได้รับมอบหมายบทบาทผู้ดูแลระบบผู้ใช้ ให้ติดต่อผู้ดูแลระบบของผู้ใช้ของคุณ For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).

**ที่อยู่ของขาย** ให้กับ - ที่อยู่ของขายให้กับ คือที่อยู่และข้อมูลที่ติดต่อขององค์กรหรือบุคคลผู้ที่รับผิดชอบบัญชีการเรียกเก็บเงิน ใบแจ้งหนี้ทั้งหมดที่สร้างขึ้นจากบัญชีการเรียกเก็บเงินจะแสดงในใบแจ้งหนี้

**ที่อยู่การเรียกเก็บเงิน** - ที่อยู่การเรียกเก็บเงินคือที่อยู่และข้อมูลที่ติดต่อขององค์กรหรือบุคคลที่จะรับผิดชอบใบแจ้งหนี้ที่สร้างขึ้นให้กับบัญชีการเรียกเก็บเงิน For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.

**เมื่อต้องการอัปเดตที่อยู่ที่ขายให้กับบัญชีการเรียกเก็บเงิน MCA**:

1. ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้ที่อยู่อีเมลซึ่งมีเจ้าของหรือบทบาทผู้สนับสนุนในบัญชีการเรียกเก็บเงินของ MCA
1. ค้นหา **การเรียกเก็บเงิน**  +  **การจัดการ** ค่าใช้จ่าย
1. คลิก **คุณสมบัติ**  >  **อัปเดตที่ขาย** ให้กับ
1. ใส่ที่อยู่ใหม่ **แล้วคลิก** บันทึก

บัญชีบางบัญชีต้องมีการตรวจสอบเพิ่มเติมก่อนจึงจะสามารถอัปเดตที่อยู่ที่ขายได้ ถ้าบัญชีของคุณต้องการการอนุมัติด้วยตนเอง คุณจะถูกขอให้ติดต่อฝ่ายสนับสนุนของ Azure

**เมื่อต้องการอัปเดตที่อยู่บัญชีการเรียกเก็บเงิน MCA**: 

1. ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้ที่อยู่อีเมลซึ่งมีเจ้าของหรือบทบาทผู้สนับสนุนบนบัญชีการเรียกเก็บเงินหรือโปรไฟล์การเรียกเก็บเงินของ MCA
1. ค้นหา **การเรียกเก็บเงิน**  +  **การจัดการ** ค่าใช้จ่าย
1. **คลิก โปรไฟล์การเรียกเก็บเงิน** และเลือกโปรไฟล์การเรียกเก็บเงินเพื่อเลือกเพื่ออัปเดตที่อยู่การเรียกเก็บเงิน
1. คลิก **คุณสมบัติ**  >  **อัปเดต** ที่อยู่
1. ใส่ที่อยู่ใหม่ **แล้วคลิก** บันทึก

**เอกสารที่แนะนา**

[เปลี่ยนข้อมูลที่ติดต่อของบัญชีการเรียกเก็บเงิน Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile)   
[อัปเดตการตั้งค่าบัญชีการเรียกเก็บเงิน](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[การเข้าใจบทบาทผู้ดูแลข้อตกลงของลูกค้า Microsoft ใน Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)