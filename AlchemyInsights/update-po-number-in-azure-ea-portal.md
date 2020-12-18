---
title: อัปเดตหมายเลข PO ใน Azure EA portal-ขั้นตอนที่แนะนำ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/17/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7290"
ms.openlocfilehash: 0388ffa5e33cca366ab02c93bb70464fb2453752
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714953"
---
# <a name="update-po-number-in-azure-ea-portal---recommended-steps"></a>อัปเดตหมายเลข PO ใน Azure EA portal-ขั้นตอนที่แนะนำ

การเปลี่ยนแปลงหมายเลขบัญชี VAT/ภาษีหรือใบสั่งซื้อ (PO) จะมีผลกับใบแจ้งหนี้ถัดไป เมื่อต้องการเปลี่ยน ID ของ VAT/ภาษีหรือหมายเลข PO เป็นใบแจ้งหนี้ที่สร้างขึ้นแล้วให้เปิดบัตรสนับสนุน ถ้าคุณมีปัญหาใดๆที่เกี่ยวข้องกับ ID VAT/ภาษีของคุณให้ติดต่อกับคู่ค้าของ Microsoft Licensing (คู่ค้าหรือที่ปรึกษาซอฟต์แวร์) พวกเขาจะติดต่อศูนย์การดำเนินการภูมิภาค (ROC) สำหรับคำถามเกี่ยวกับ ID VAT/ภาษีของคุณ 

พอร์ทัล EA ของ Azure จะสร้างหมายเลข PO เริ่มต้นโดยอัตโนมัติยกเว้นว่าผู้ดูแลระบบ EA ตั้งค่าก่อนวันที่ในใบแจ้งหนี้ ในฐานะผู้ดูแลระบบ EA (การลงทะเบียนโดยตรง)/ผู้ดูแลระบบคู่ค้า (การลงทะเบียนทางอ้อม) คุณสามารถอัปเดตหมายเลข PO ในพอร์ทัล EA ของ Azure ได้ คุณสามารถอัพเดตหมายเลข PO ได้ตลอดเวลาก่อนที่จะมีการสร้างใบแจ้งหนี้สำหรับระยะเวลาการเรียกเก็บเงินปัจจุบันและไม่เกินเจ็ดวันหลังจากได้รับอีเมลแจ้งเตือนเกี่ยวกับใบแจ้งหนี้อัตโนมัติ    

เมื่อต้องการอัปเดตหมายเลข PO:

1. ลงชื่อเข้าใช้[พอร์ทัล EA](https://ea.azure.com/)
1. ในบานหน้าต่างด้านซ้ายให้คลิก **รายงาน**
1. ที่ด้านบนของหน้าให้คลิก **สรุปการใช้งาน** แล้วเลือกระยะเวลาที่เกี่ยวข้องจากเมนูดรอปดาวน์
1. คลิก **ดู/แก้ไขหมายเลข PO**
1. ใส่หมายเลข PO ใหม่แล้วคลิก **บันทึก**

**เอกสารที่แนะนำ** 

- [ใบแจ้งหนี้การลงทะเบียนขององค์กร Azure](https://docs.microsoft.com/azure/billing/billing-ea-portal-enrollment-invoices) 
- [ทำความเข้าใจใบเรียกเก็บเงินข้อตกลงองค์กร Azure ของคุณ](https://docs.microsoft.com/azure/billing/billing-understand-your-bill-ea)  
- [ทำความเข้าใจเกี่ยวกับบทบาทขององค์กร Azure](https://docs.microsoft.com/azure/billing/billing-understand-your-bill-ea) 
- [สร้างผู้ดูแลระบบขององค์กรอื่น (ผู้ดูแลระบบ EA)](https://docs.microsoft.com/azure/cost-management-billing/manage/ea-portal-administration#create-another-enterprise-administrator) 
