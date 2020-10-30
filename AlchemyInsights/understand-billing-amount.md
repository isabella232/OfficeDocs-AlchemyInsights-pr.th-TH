---
title: ทำความเข้าใจเกี่ยวกับจำนวนเงินที่เรียกเก็บเงิน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003554"
- "6680"
ms.openlocfilehash: f48ee1e36909515bf81df1ebeb367f91e9a1c9ca
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808401"
---
# <a name="understand-billing-amount"></a>ทำความเข้าใจเกี่ยวกับจำนวนเงินที่เรียกเก็บเงิน

**ลูกค้า Led (WD):**

- เพื่อช่วยในการตรวจสอบและทำความเข้าใจใบเรียกเก็บเงินของคุณโปรดดู:[บทช่วยสอน: ตรวจสอบใบเรียกเก็บเงินของคุณแต่ละ](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support)รายการ
- ทำความเข้าใจเกี่ยวกับข้อกำหนดในใบแจ้งหนี้ของคุณ: [คำอธิบายเงื่อนไขใบแจ้งหนี้ของ Azure](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- ทำความเข้าใจเกี่ยวกับข้อกำหนดของค่าใช้จ่ายในการใช้งาน Azure: [คำอธิบายเกี่ยวกับการใช้งาน](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-usage?WT.mc_id=Portal-Microsoft_Azure_Support)
- เมื่อต้องการรับ PDF ของใบแจ้งหนี้ของคุณและสำเนาของไฟล์การใช้งานรายละเอียดของคุณ ( CSV): [รับข้อมูลใบแจ้งหนี้และการใช้งาน](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**หมายเหตุ** : ถ้าคุณยกเลิกการสมัครใช้งาน/ทรัพยากรของคุณในช่วงกลางของรอบการเรียกเก็บเงินของคุณคุณอาจยังเห็นค่าใช้จ่ายที่ใช้สำหรับการใช้งานในเดือนก่อนหน้านี้ ตัวอย่างเช่นถ้ารอบการเรียกเก็บเงินของคุณมาจากวันที่26ของเดือนจนถึง25ของเดือนถัดไป & คุณระงับการสมัครใช้งานบน23ซึ่งเป็นวันที่28วันลงในรอบการเรียกเก็บเงินเดือนมิถุนายนคุณอาจเห็นค่าใช้จ่ายสำหรับการใช้งาน28วัน ถ้าคุณเห็นค่าใช้จ่ายแม้ว่าการยกเลิกการสมัครใช้งานโปรดตรวจสอบให้แน่ใจว่าคุณไม่มีแผนการสนับสนุนอื่นๆที่ทำให้เกิดค่าใช้จ่าย ถ้าคุณทำเช่นนั้นโปรดไปข้างหน้าและยกเลิกแผน

**ข้อตกลงลูกค้าของ Microsoft (MCA):**

[วิธีการตรวจสอบการเข้าถึงข้อตกลงลูกค้าของ Microsoft ใช่หรือไม่](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)

- เพื่อช่วยในการตรวจสอบและทำความเข้าใจใบเรียกเก็บเงินของคุณโปรดดู: [บทช่วยสอน: ตรวจทานใบแจ้งหนี้ข้อตกลงของลูกค้า Microsoft ของคุณ](https://docs.microsoft.com/azure/cost-management-billing/understand/review-customer-agreement-bill?WT.mc_id=Portal-Microsoft_Azure_Support)
- ทำความเข้าใจเกี่ยวกับข้อกำหนดในใบแจ้งหนี้ของคุณ: [คำอธิบายเกี่ยวกับใบแจ้งหนี้ข้อตกลงของลูกค้าของ Microsoft](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-understand-your-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- ทำความเข้าใจเกี่ยวกับข้อกำหนดในการใช้งาน Azure: [คำอธิบายข้อตกลงการใช้งานข้อตกลงของลูกค้าของ Microsoft](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-understand-your-usage?WT.mc_id=Portal-Microsoft_Azure_Support)
- ถ้าคุณมี [ข้อตกลงลูกค้าของ Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)คุณสามารถดาวน์โหลดการใช้งานใน [พอร์ทัล Azure](https://portal.azure.com/)ได้

**ข้อตกลงคู่ค้าของไมโครซอฟท์ (MPA):**

- เพื่อช่วยในการตรวจสอบและทำความเข้าใจใบเรียกเก็บเงินของคุณโปรดดู: [บทช่วยสอน: ตรวจทานใบแจ้งหนี้ข้อตกลงของคู่ค้าของ Microsoft](https://docs.microsoft.com/azure/cost-management-billing/understand/review-partner-agreement-bill?WT.mc_id=Portal-Microsoft_Azure_Support)
- ทำความเข้าใจเกี่ยวกับข้อกำหนดในใบแจ้งหนี้ของคุณ: [คำอธิบายในใบแจ้งหนี้ข้อตกลงเกี่ยวกับคู่ค้าของไมโครซอฟท์](https://docs.microsoft.com/azure/cost-management-billing/understand/mpa-invoice-terms?WT.mc_id=Portal-Microsoft_Azure_Support)

**ข้อตกลงขององค์กร (EA)**

- เพื่อช่วยตรวจสอบและทำความเข้าใจใบเรียกเก็บเงินของคุณโปรดดูที่: ทำความ [เข้าใจใบเรียกเก็บเงินข้อตกลงองค์กร Azure ของคุณ](https://docs.microsoft.com/azure/cost-management-billing/understand/review-enterprise-agreement-bill?WT.mc_id=Portal-Microsoft_Azure_Support)
- ถ้าคุณเป็นลูกค้า Azure ที่มีข้อตกลงขององค์กร (ลูกค้า EA) คุณจะไม่สามารถดาวน์โหลดใบแจ้งหนี้ขององค์กรของคุณได้ ใบแจ้งหนี้จะถูกส่งไปยังผู้ใดก็ตามที่ตั้งค่าไว้เพื่อรับใบแจ้งหนี้สำหรับการลงทะเบียนคุณสามารถดาวน์โหลดการใช้งานใน [พอร์ทัล Azure](https://portal.azure.com/)ได้

ตรวจทานใบแจ้งหนี้ของบริการขีด:

- ลงชื่อเข้าใช้ใน **เว็บไซต์องค์กร** เลือก **รายงาน**
- ที่มุมบนขวาของแท็บให้สลับมุมมองจาก **M** เป็น **C** และตรงกับช่วงเวลาบนใบแจ้งหนี้
- จำนวน **การใช้งาน** ทั้งหมดควรตรงกับจำนวนที่ **เพิ่ม** ขึ้นทั้งหมดบนใบแจ้งหนี้ขีดบริการของคุณ
- ไปที่ **ดาวน์โหลดการใช้งาน > การดาวน์โหลดรายงานขั้นสูง** เพื่อรับข้อมูลเพิ่มเติมเกี่ยวกับ **หมายเหตุ** ค่าใช้จ่ายของคุณ: รายงานนี้ไม่รวมภาษีค่าธรรมเนียมสำหรับการจองหรือค่าใช้จ่ายในตลาด

**Azure Marketplace**

- เรียนรู้เพิ่มเติมเกี่ยวกับวิธีการเรียกเก็บเงินของบริษัทอื่น: การ [เรียกเก็บเงินของ Azure Marketplace](https://docs.microsoft.com/azure/billing/billing-understand-your-azure-marketplace-charges?WT.mc_id=Portal-Microsoft_Azure_Support)

ตรวจทานใบแจ้งหนี้ของ Marketplace:

เปรียบเทียบผลรวมของ Azure Marketplace ของคุณบนรายงาน > สรุปการใช้งานในเว็บไซต์องค์กรกับใบแจ้งหนี้ของตลาดของคุณ ใบแจ้งหนี้ของ marketplace มีไว้สำหรับการซื้อและการใช้ Azure Marketplace เท่านั้น จำนวนของข้อมูลสรุปการใช้งานจะไม่รวมภาษี

- ลงชื่อเข้าใช้ใน **เว็บไซต์องค์กร** เลือก **รายงาน**
- ที่มุมบนขวาของแท็บให้สลับมุมมองจาก **M** เป็น **C** และตรงกับช่วงเวลาบนใบแจ้งหนี้
- ผลรวมของ **Azure marketplace** ควรตรงกับ **ยอดขายรวม** บนใบแจ้งหนี้ของ Marketplace ของคุณ
- ไปที่ **ดาวน์โหลดการใช้งาน** เพื่อรับข้อมูลเพิ่มเติมเกี่ยวกับค่าใช้จ่ายที่ใช้สำหรับการใช้งานของคุณ ภายใต้ **ค่าบริการมาร์เก็ต** ให้เลือก **ดาวน์โหลด****หมายเหตุ** : รายงานนี้ไม่รวมภาษีหรือแสดงการซื้อครั้งเดียว

**ผู้ให้บริการโซลูชัน Cloud (CSP)**

- เรียนรู้เพิ่มเติมเกี่ยวกับวิธีการทำงานของการเรียกเก็บเงินในโปรแกรมผู้ให้บริการโซลูชันของ Azure Cloud (Azure CSP): การ [เรียกเก็บเงินของ AZURE CSP](https://docs.microsoft.com/azure/cloud-solution-provider/billing/azure-csp-billing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)
- เรียนรู้เกี่ยวกับการอ่านและทำความเข้าใจเกี่ยวกับการเรียกเก็บเงินของคุณ CSP: [ใบแจ้งหนี้ของ AZURE CSP](https://docs.microsoft.com/azure/cloud-solution-provider/billing/azure-csp-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนำ**

- เรียนรู้วิธีการป้องกันค่าใช้จ่ายที่ไม่คาดคิดและควบคุมค่าใช้จ่ายของคุณ: [ป้องกันค่าใช้จ่ายที่ไม่คาดคิด](https://docs.microsoft.com/azure/cost-management-billing/manage/getting-started?WT.mc_id=Portal-Microsoft_Azure_Support)
- ตั้งค่าการเรียกเก็บเงินหรือการแจ้งเตือนเครดิตเพื่อตรวจสอบและจัดการกิจกรรมการเรียกเก็บเงินสำหรับบัญชีผู้ใช้ของคุณ: [ตั้งค่าการแจ้งเตือนการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/costs/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ทำความเข้าใจวงเงินใช้จ่ายของ Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
- ทำความเข้าใจเกี่ยวกับการเรียกเก็บเงิน Azure ของคุณสำหรับค่าบริการภายนอก: [วิธีการเรียกเก็บเงินจากบริการภายนอก](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-azure-marketplace-charges?WT.mc_id=Portal-Microsoft_Azure_Support)
- [คำถามที่ถามบ่อยเกี่ยวกับบัญชีผู้ใช้ Azure ฟรี](https://azure.microsoft.com/free/free-account-faq/)
- [ทำความเข้าใจเกี่ยวกับบทบาทการดูแลข้อตกลงขององค์กร Azure ใน Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-ea-roles?WT.mc_id=Portal-Microsoft_Azure_Support)