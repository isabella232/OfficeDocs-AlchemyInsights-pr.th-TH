---
title: อัปเดตหมายเลข PO - EA รุ่นดั้งเดิม - ขั้นตอนที่แนะน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/09/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9004166"
- "7322"
ms.openlocfilehash: 7c3ee469107e9ab85dcf56450167cc2e47b2c8b79253d45b1a362959a869ba24
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53908513"
---
# <a name="update-purchase-order-number---legacy-ea---recommended-steps"></a>อัปเดตหมายเลขใบสั่งซื้อ - EA ดั้งเดิม - ขั้นตอนที่แนะน

การเปลี่ยนแปลงหมายเลขใบสั่งซื้อ (PO) จะมีผลในใบแจ้งหนี้ถัดไป เมื่อต้องการเปลี่ยนหมายเลข PO บนใบแจ้งหนี้ที่สร้างไว้แล้ว ให้เปิดตั๋วการสนับสนุน 

พอร์ทัล Azure EA จะสร้างหมายเลข PO เริ่มต้นโดยอัตโนมัติ เว้นแต่ผู้ดูแลระบบ EA จะตั้งค่าก่อนวันที่ในใบแจ้งหนี้ ในฐานะผู้ดูแลระบบ EA (การลงทะเบียนโดยตรง) / ผู้ดูแลระบบคู่ค้า (การลงทะเบียนทางอ้อม) คุณสามารถอัปเดตหมายเลข PO ในพอร์ทัล Azure EA เมื่อต้องการอัปเดตหมายเลข PO:

1. ลงชื่อเข้าใช้พอร์ทัล EA
2. **คลิก** รายงาน ทางด้านซ้าย
3. **คลิก สรุป** การใช้งาน ที่ด้านบนของหน้า
4. เลือกช่วงเวลาที่เกี่ยวข้องจากรายการดรอปดาวน์
5. คลิก **ดู/แก้ไขหมายเลข** PO
6. ป้อนหมายเลข PO ใหม่ **แล้วคลิก** บันทึก

คุณสามารถอัปเดตหมายเลข PO ได้ตลอดเวลาก่อนที่จะสร้างใบแจ้งหนี้ในช่วงเวลาการเรียกเก็บเงินปัจจุบัน และสูงสุดเจ็ดวันหลังจากได้รับอีเมลการแจ้งเตือนใบแจ้งหนี้อัตโนมัติ 

**เอกสารที่แนะนา**

- [ใบแจ้งหนี้การลงทะเบียนองค์กรของ Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-enrollment-invoices) 
- [เข้าใจใบเรียกเก็บเงิน Azure Enterprise Agreementของคุณ](https://docs.microsoft.com/azure/cost-management-billing/understand/review-enterprise-agreement-bill)  
- [การเข้าใจบทบาท Azure Enterprise](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-ea-roles#add-a-new-enterprise-administrator) 
- [สร้างผู้ดูแลระบบขององค์กรอื่น (ผู้ดูแลระบบ EA)](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-administration#create-another-enterprise-administrator)
