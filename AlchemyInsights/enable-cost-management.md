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
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003588"
---
# <a name="enable-cost-management"></a>เปิดใช้งานการจัดการต้นทุน

**'ค่าใช้จ่ายถูกปิดใช้งานในองค์กรของคุณ' หมายถึงอะไร**

องค์กรที่ใช้บัญชี Enterprise Agreement (EA) หรือ Microsoft Customer Agreement (MCA) สามารถปิดใช้งานการเข้าถึงข้อมูลต้นทุนและข้อมูลราคาได้

หลังจากเข้าสู่ระบบพอร์ทัล Azure แล้ว พวกเขาจะสามารถใช้ API การเรียกเก็บเงินเพื่อรับใบแจ้งหนี้ (เมื่อเข้าร่วม) และรายละเอียดการใช้งานโดยทางโปรแกรมได้

**วิธีการอนุญาตให้ผู้ใช้เพิ่มเติมเข้าถึงใบแจ้งหนี้**

1. ไปที่ **Blade การสมัครใช้งาน** ในพอร์ทัล Azure
2. **เลือก ใบแจ้งหนี้****แล้วเข้าถึง** ใบแจ้งหนี้
3. เปิดการเข้าถึงตามด้วยการบันทึกการเปลี่ยนแปลง เพื่ออนุญาตให้ผู้ใช้ที่มีบทบาทในการสมัครใช้งานสามารถดาวน์โหลดใบแจ้งหนี้ได้

> [!NOTE]
> ผู้ดูแลระบบบัญชียังสามารถกําหนดค่าให้ส่งใบแจ้งหนี้ทางอีเมลได้ เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู รับใบแจ้งหนี้ใน](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)อีเมล

**วิธีเพิ่มผู้ใช้ลงในบทบาทโปรแกรมอ่านการเรียกเก็บเงิน**

1. ไปที่ **Blade การสมัครใช้งาน** ในพอร์ทัล Azure
2. เลือก **ตัวควบคุมการเข้าถึง (IAM)** **แล้วคลิก** เพิ่ม
3. เลือก **ตัว** อ่านการเรียกเก็บเงิน **ในหน้า เลือก** บทบาท
4. พิมพ์อีเมลของผู้ใช้ที่คุณต้องการเชิญ แล้วคลิก ตกลง **เพื่อ** ส่งคําเชิญ
5. Follow instructions provided in the invite email to log in as a billing reader. หากต้องการข้อมูลเพิ่มเติม โปรดดู [ให้สิทธิ์การเข้าถึง](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)การเรียกเก็บเงิน

**เอกสารที่แนะนา**

- [เปิดใช้งานมุมมอง DA และ EA ผ่านพอร์ทัล EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [ต้นทุนที่รวมอยู่ในการจัดการต้นทุน](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [ข้อเสนอ Microsoft Azure ที่สนับสนุน](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [ตรวจสอบต้นทุนในการวิเคราะห์ต้นทุน](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [ให้การเข้าถึงข้อมูลการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ตรวจสอบการเข้าถึงข้อตกลงของลูกค้า Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






