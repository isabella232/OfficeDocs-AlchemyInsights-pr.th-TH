---
title: การยกเลิกการจอง
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819711"
---
# <a name="cancelling-reservation"></a>การยกเลิกการจอง

- **บริการตนเอง:** คุณสามารถยกเลิกหรือเปลี่ยนอินสแตนซ์สงวนด้วยตนเองได้โดยใช้ [พอร์ทัล Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) เลือกการจองและคลิกขอคืนเงินหรือเปลี่ยน โปรดทราบว่าคุณต้องมีสิทธิ์ในการเข้าถึงใน การสั่งซื้อการจอง เพื่อแลกเปลี่ยนหรือคืนเงิน Access to only reservation will not let you proceed with refund or exchange. สอบถามเจ้าของใบสั่งซื้อการจองเพื่อให้เจ้าของมีสิทธิ์เข้าถึงใบสั่งซื้อที่จองได้
- **นโยบาย Exchange:** คุณสามารถแลกเปลี่ยนการจองการจองประเภทเดียวกันได้ - ไม่มีข้อ **ห้าม** ในการแลกเปลี่ยนการจอง ข้อผูกมัดรวมที่มีการจองใหม่ควรมากกว่าผลรวมของยอดเงินคืนของการจองที่เปลี่ยนแล้วและการจ่ายเงินรายเดือนในอนาคต (ถ้ามี)
- **นโยบายการคืนเงิน:** ผลรวมของการคืนเงินและการยอดเงินที่ยกเลิกในอนาคตจะต้องไม่เกิน $50,000 USD ในหน้าต่างเลื่อนล่วงหน้า 12 เดือน ขณะนี้ **เราไม่ได้ชาร์จค่าปรับใดๆ กับ** การคืนเงิน แต่สามารถเรียกเก็บเงินจากการคืนเงินในอนาคตได้  
    **ข้อยกเว้น:** การแลกเปลี่ยนด้วยตนเองและการยกเลิกความสามารถยังไม่พร้อมใช้งานกับลูกค้าของหน่วยงานภาครัฐของสหรัฐอเมริกา
- **การสนับสนุน API / PS / CLI** ไม่พร้อมให้ใช้งานในการยกเลิกและการคืนเงินการแลกเปลี่ยนแบบบริการ [ตนเองและการคืนเงินของ Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- การแลกเปลี่ยนด้วยตนเองและการยกเลิกความสามารถยังไม่พร้อมใช้งานกับลูกค้าของหน่วยงานภาครัฐของสหรัฐอเมริกา ชนิดการสมัครใช้งานอื่นๆ ของภาครัฐของสหรัฐอเมริกา รวมถึง Pay-As-You-Go และ CSP ได้รับการสนับสนุน

เรียนรู้เพิ่มเติม : [วิธีการประมวลผลทรานแซคชันการส่งคืนและแลกเปลี่ยน](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
เรียนรู้เพิ่มเติม: [นโยบายการแลกเปลี่ยนและการคืนเงิน](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
ข้อสงสัยอื่นๆ: [เยี่ยมชมเอกสารอินสแตนซ์ที่สงวนไว้](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange อินสแตนซ์สงวนที่มีอยู่ (บริการตนเอง)**

คุณสามารถแลกเปลี่ยนการจองเพื่อจองประเภทเดียวกันได้ คุณยังสามารถคืนเงินการจองได้ สูงสุดถึง $50,000 USD ต่อปี ถ้าคุณไม่ต้องการแล้ว การแลกเปลี่ยนด้วยตนเองและการยกเลิกความสามารถยังไม่พร้อมใช้งานกับลูกค้าของหน่วยงานภาครัฐของสหรัฐอเมริกา ชนิดการสมัครใช้งานอื่นๆ ของภาครัฐของสหรัฐอเมริกา รวมถึง Pay-As-You-Go และ CSP ได้รับการสนับสนุน คุณต้องมีสิทธิ์การเข้าถึงใน การสั่งซื้อจอง เพื่อแลกเปลี่ยนหรือคืนเงินเป็นการจองที่มีอยู่

ขั้นตอนต่อไปนี้จะเป็นแนวทางเกี่ยวกับกระบวนการในการทรานแซคชันให้เสร็จสมบูรณ์

1. ลงชื่อเข้าใช้พอร์ทัล [Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)ของคุณ เลือกการจองที่คุณต้องการคืนเงิน แล้วคลิก **Exchange**
2. เลือกผลิตภัณฑ์ VM ที่คุณต้องการซื้อและพิมพ์ปริมาณ ตรวจสอบให้แน่ใจว่าผลรวมการซื้อใหม่มากกว่าผลรวมการส่งคืน [ให้ระบุขนาดที่เหมาะสมก่อนที่คุณจะซื้อ](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. ตรวจทานและกรอกข้อมูลทรานแซคชัน

**การขอคืนเงินกรณีสงวน**

เมื่อต้องการคืนเงินในการจอง ให้ไปที่ รายละเอียด **การจองห้อง** แล้วคลิก **คืนเงิน**

**การคืนเงินตามการจัดอันดับโปร:**

**ตัวอย่างการขอคืนเงินและการแลกเปลี่ยนของ Pro-ration และความต้องการขั้นต่่**  
ตัวอย่างการจองล่วงหน้า:

- คุณซื้อ RI ระยะเวลาหนึ่งปีราคา $120 ในวันที่ 1 มกราคม
- ในวันที่ 7 เมษายนที่คุณต้องการคืนเงินหรือเปลี่ยนการจองนี้
- เนื่องจากการจองอยู่เป็นเวลา 97 วัน คุณจะได้รับ (1-97/365) * $120 กลับไป (เช่น $88.1) ขณะนี้ยังไม่มีค่าปรับค่าปรับในการคืนเงิน
- ถ้าแลกเปลี่ยน การซื้อใหม่ของคุณควรมากกว่า $88.1
- ไม่มีการได้รับค่าปรับในการคืนเงินในปัจจุบัน

**ตัวอย่างการจองแผนการเรียกเก็บเงิน:**

- คุณซื้อ RI ระยะเวลาหนึ่งปีราคา $10 ต่อเดือน
- ในวันที่ 7 เมษายนที่คุณต้องการคืนเงินหรือเปลี่ยนการจองนี้
- เนื่องจากมีการอัปเดตล่าสุด 7 วัน คุณจะได้รับ (1-7/31) * $10 กลับมา (เช่น $7.74)
- การจ่ายเงินในอนาคตที่ถูกยกเลิกคือ $ 80 ขณะนี้ยังไม่มีค่าปรับค่าปรับในการคืนเงิน
- การยกเลิกนี้จะหักเงิน $87.74 ออกจากขีดจํากัดการคืนเงิน $50,000
- ถ้าแลกเปลี่ยน มูลค่ารวมของการซื้อใหม่ควรมากกว่า $87.74

**เอกสารที่แนะนา**

- [วิธีการประมวลผลทรานแซคชันการส่งคืนและแลกเปลี่ยน](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [นโยบายการแลกเปลี่ยนและการคืนเงิน](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)