---
title: เปิดใช้งานการจัดการต้นทุน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678774"
---
# <a name="enable-cost-management"></a>เปิดใช้งานการจัดการต้นทุน

**' ค่าใช้จ่าย ' ถูกปิดใช้งานสำหรับองค์กรของคุณอย่างไร**

องค์กรที่ใช้บัญชีข้อตกลงขององค์กร (EA) หรือบัญชีผู้ใช้ข้อตกลงลูกค้าของ Microsoft (MCA) สามารถปิดใช้งานการเข้าถึงข้อมูลต้นทุนและข้อมูลการกำหนดราคาได้

หลังจากที่คุณเข้าสู่ระบบไปยังพอร์ทัล Azure พวกเขาสามารถใช้ APIs การเรียกเก็บเงินเพื่อรับใบแจ้งหนี้ได้โดยทางโปรแกรม (เมื่อมีการเข้าร่วม) และรายละเอียดการใช้งาน

**วิธีการอนุญาตให้ผู้ใช้เพิ่มเติมในการเข้าถึงใบแจ้งหนี้**

1. ไปที่ **ใบมีดการสมัคร** ใช้งานในพอร์ทัล Azure
2. เลือก **ใบแจ้งหนี้** แล้ว **เข้าถึงใบแจ้งหนี้**
3. เปิดใช้งานการเข้าถึงตามด้วยการบันทึกการเปลี่ยนแปลงเพื่ออนุญาตให้ผู้ใช้ในการสมัครใช้งาน-ลักษณะบทบาทในการดาวน์โหลดใบแจ้งหนี้

> [!NOTE]
> ผู้ดูแลระบบบัญชียังสามารถกำหนดค่าให้มีใบแจ้งหนี้ที่ส่งผ่านทางอีเมล เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[รับใบแจ้งหนี้ของคุณในอีเมล](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**วิธีเพิ่มผู้ใช้ลงในบทบาทผู้อ่านการเรียกเก็บเงิน**

1. ไปที่ **ใบมีดการสมัคร** ใช้งานในพอร์ทัล Azure
2. เลือก **ตัวควบคุมการเข้าถึง (IAM)** แล้วคลิก **เพิ่ม**
3. เลือกตัว **อ่านการเรียกเก็บเงิน** ในหน้า **เลือกบทบาท**
4. พิมพ์อีเมลของผู้ใช้ที่คุณต้องการเชิญแล้วคลิก **ตกลง** เพื่อส่งคำเชิญ
5. ทำตามคำแนะนำที่ให้ไว้ในอีเมลเชิญเพื่อเข้าสู่ระบบในฐานะผู้อ่านการเรียกเก็บเงิน สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ให้สิทธิ์การเข้าถึงการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**เอกสารที่แนะนำ**

- [เปิดใช้งานมุมมอง DA และอ่าวผ่านทาง EA portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [ค่าใช้จ่ายที่รวมอยู่ในการจัดการต้นทุน](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [ข้อเสนอ Microsoft Azure ที่ได้รับการสนับสนุน](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [ตรวจทานต้นทุนในการวิเคราะห์ต้นทุน](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [ให้สิทธิ์การเข้าถึงข้อมูลการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ตรวจสอบการเข้าถึงข้อตกลงลูกค้าของ Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






