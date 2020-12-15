---
title: อัปเดตหมายเลข PO-ขั้นตอนที่แนะนำ EA
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
ms.openlocfilehash: ef1e5f52cb26542892199694309fb2b0df551997
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679595"
---
# <a name="update-purchase-order-number---legacy-ea---recommended-steps"></a>อัปเดตหมายเลขใบสั่งซื้อ-ขั้นตอนที่แนะนำของ EA แบบดั้งเดิม

การเปลี่ยนแปลงหมายเลขใบสั่งซื้อ (PO) จะมีผลกับใบแจ้งหนี้ถัดไป เมื่อต้องการเปลี่ยนหมายเลข PO บนใบแจ้งหนี้ที่สร้างขึ้นแล้วให้เปิดบัตรสนับสนุน 

พอร์ทัล EA ของ Azure จะสร้างหมายเลข PO เริ่มต้นโดยอัตโนมัติยกเว้นว่าผู้ดูแลระบบ EA ตั้งค่าก่อนวันที่ในใบแจ้งหนี้ ในฐานะผู้ดูแลระบบ EA (การลงทะเบียนโดยตรง)/ผู้ดูแลระบบคู่ค้า (การลงทะเบียนทางอ้อม) คุณสามารถอัปเดตหมายเลข PO ในพอร์ทัล EA ของ Azure ได้ เมื่อต้องการอัปเดตหมายเลข PO:

1. ลงชื่อเข้าใช้พอร์ทัล EA
2. คลิก **รายงาน** ทางด้านซ้ายมือ
3. คลิก **สรุปการใช้งาน** ที่ด้านบนของหน้า
4. เลือกช่วงเวลาที่เกี่ยวข้องจากรายการดรอปดาวน์
5. คลิก **ดู/แก้ไขหมายเลข PO**
6. ใส่หมายเลข PO ใหม่แล้วคลิก **บันทึก**

คุณสามารถอัพเดตหมายเลข PO ได้ตลอดเวลาก่อนที่จะมีการสร้างใบแจ้งหนี้สำหรับช่วงเวลาการเรียกเก็บเงินปัจจุบันและไม่เกิน7วันหลังจากที่ได้รับอีเมลแจ้งให้ทราบเกี่ยวกับใบแจ้งหนี้อัตโนมัติ 

**เอกสารที่แนะนำ**

- [ใบแจ้งหนี้การลงทะเบียนขององค์กร Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-enrollment-invoices) 
- [ทำความเข้าใจใบเรียกเก็บเงินข้อตกลงองค์กร Azure ของคุณ](https://docs.microsoft.com/azure/cost-management-billing/understand/review-enterprise-agreement-bill)  
- [ทำความเข้าใจเกี่ยวกับบทบาทขององค์กร Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-ea-roles#add-a-new-enterprise-administrator) 
- [สร้างผู้ดูแลระบบขององค์กรอื่น (ผู้ดูแลระบบ EA)](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-administration#create-another-enterprise-administrator)
