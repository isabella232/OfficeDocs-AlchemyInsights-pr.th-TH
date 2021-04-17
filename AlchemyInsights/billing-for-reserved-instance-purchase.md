---
title: การเรียกเก็บเงินกรณีการเหมาจ่ายล่วงหน้า
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820341"
---
# <a name="billing-for-reserved-instance-purchase"></a>การเรียกเก็บเงินกรณีการเหมาจ่ายล่วงหน้า

การซื้ออินสแตนซ์แบบเหมาจ่ายจะถูกเรียกเก็บเงินจากวิธีการเงินที่ผูกกับการสมัครใช้งานที่คุณเลือกเมื่อซื้อ ชนิดการสมัครใช้งานต้องเป็นข้อตกลงขององค์กร (หมายเลขข้อเสนอ: MS-AZR-0017P), Pay-as-You-Go (หมายเลขข้อเสนอ: MS-AZR-0003P), ข้อตกลงของลูกค้า Microsoft หรือ CSP

- For an enterprise subscription, the charges are deducted from the enrollment's monetary commitment balance or charged as overage
- For Pay-As-You-Go subscription, the charges are billed to the credit card or invoice payment method on the subscription

**การยกเลิกการจอง**

- **บริการตนเอง:** คุณสามารถยกเลิกหรือเปลี่ยนอินสแตนซ์สงวนด้วยตนเองได้โดยใช้ [พอร์ทัล Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) เลือกการจองและคลิกขอคืนเงินหรือเปลี่ยน โปรดทราบว่าคุณต้องมีสิทธิ์ในการเข้าถึงใน การสั่งซื้อการจอง เพื่อแลกเปลี่ยนหรือคืนเงิน Access to only reservation will not let you proceed with refund or exchange. สอบถามเจ้าของใบสั่งซื้อการจองเพื่อให้เจ้าของมีสิทธิ์เข้าถึงใบสั่งซื้อที่จองได้
- **นโยบาย Exchange:** คุณสามารถแลกเปลี่ยนการจองการจองประเภทเดียวกันได้ - ไม่มีข้อ **ห้าม** ในการแลกเปลี่ยนการจอง ข้อผูกมัดรวมที่มีการจองใหม่ควรมากกว่าผลรวมของยอดเงินคืนของการจองที่เปลี่ยนแล้วและการจ่ายเงินรายเดือนในอนาคต (ถ้ามี)
- **นโยบายการคืนเงิน:** ผลรวมของการคืนเงินและการยอดเงินที่ยกเลิกในอนาคตจะต้องไม่เกิน $50,000 USD ในหน้าต่างเลื่อนล่วงหน้า 12 เดือน ขณะนี้ **เราไม่ได้ชาร์จค่าปรับใดๆ กับ** การคืนเงิน แต่สามารถเรียกเก็บเงินจากการคืนเงินในอนาคตได้

**ข้อยกเว้น:** การแลกเปลี่ยนด้วยตนเองและการยกเลิกความสามารถยังไม่พร้อมใช้งานกับลูกค้าของหน่วยงานภาครัฐของสหรัฐอเมริกา

- **การสนับสนุน API / PS / CLI** ไม่พร้อมให้ใช้งานในการยกเลิกและการคืนเงินการแลกเปลี่ยนแบบบริการ [ตนเองและการคืนเงินของ Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- การแลกเปลี่ยนด้วยตนเองและการยกเลิกความสามารถยังไม่พร้อมใช้งานกับลูกค้าของหน่วยงานภาครัฐของสหรัฐอเมริกา ชนิดการสมัครใช้งานอื่นๆ ของภาครัฐของสหรัฐอเมริกา รวมถึง Pay-As-You-Go และ CSP ได้รับการสนับสนุน

เรียนรู้เพิ่มเติม: [วิธีการประมวลผลการส่งคืนและแลกเปลี่ยนธุรกรรม](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) เรียนรู้เพิ่มเติม : นโยบาย [Exchange และการคืนเงิน ข้อ](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) ถามอื่นๆ: [เอกสารอินสแตนซ์ที่สงวนไว้](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange อินสแตนซ์สงวนที่มีอยู่ (บริการตนเอง)**

คุณสามารถแลกเปลี่ยนการจองเพื่อจองประเภทเดียวกันได้ คุณยังสามารถคืนเงินการจองได้ สูงสุดถึง $50,000 USD ต่อปี ถ้าคุณไม่ต้องการแล้ว การแลกเปลี่ยนด้วยตนเองและการยกเลิกความสามารถยังไม่พร้อมใช้งานกับลูกค้าของหน่วยงานภาครัฐของสหรัฐอเมริกา ชนิดการสมัครใช้งานอื่นๆ ของภาครัฐของสหรัฐอเมริกา รวมถึง Pay-As-You-Go และ CSP ได้รับการสนับสนุน คุณต้องมีสิทธิ์การเข้าถึงใน การสั่งซื้อจอง เพื่อแลกเปลี่ยนหรือคืนเงินเป็นการจองที่มีอยู่

ขั้นตอนต่อไปนี้จะเป็นแนวทางเกี่ยวกับกระบวนการในการทรานแซคชันให้เสร็จสมบูรณ์

1.เข้าสู่ระบบพอร์ทัล [Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)ของคุณ เลือกการจองที่คุณต้องการคืนเงิน แล้วคลิก **Exchange** 2 เลือกผลิตภัณฑ์ VM ที่คุณต้องการซื้อและพิมพ์ปริมาณ ตรวจสอบให้แน่ใจว่าผลรวมการซื้อใหม่มากกว่าผลรวมการส่งคืน [ให้ระบุขนาดที่เหมาะสมก่อนที่คุณจะ](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)ซื้อ
3.ตรวจทานและเสร็จสิ้นการทรานแซคชัน

**การขอคืนเงินกรณีสงวน**

เมื่อต้องการคืนเงินในการจอง ให้ไปที่ รายละเอียด **การจองห้อง** แล้วคลิก **คืนเงิน**

**การคืนเงินตามการจัดอันดับโปร:**

**ตัวอย่างการขอคืนเงินและการแลกเปลี่ยนของ Pro-ration** และความต้องการขั้นต่่ ตัวอย่างการจองล่วงหน้า:

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

**ไม่สามารถดูใบแจ้งหนี้ของรอบการเรียกเก็บเงินล่าสุด**

สาเหตุบางประการที่อาจเป็นไปได้ที่คุณอาจไม่เห็นใบแจ้งหนี้:

- คุณมีจํานวนเครดิตรายเดือนกับการสมัครใช้งานของคุณที่ไม่เกินหรือมีรุ่นทดลองใช้ฟรี ใบแจ้งหนี้จะถูกสร้างขึ้นเมื่อคุณค้างเงินเท่านั้น
- ภายในเวลาไม่ถึง 30 วันนับจากวันที่คุณสมัครใช้งาน Azure
- ยังไม่มีการสร้างใบแจ้งหนี้ รอจนถึงวันที่สิ้นสุดของรอบการเรียกเก็บเงิน
- ถ้าคุณไม่ได้เป็นผู้ดูแลบัญชี ใบแจ้งหนี้ที่เก่ากว่าอาจไม่พร้อมให้คุณใช้งาน

**ดาวน์โหลดใบแจ้งหนี้ของคุณจากพอร์ทัล Azure (.pdf)**

- เลือกการสมัครใช้งานของคุณ [จากหน้าการสมัครใช้งาน](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ในพอร์ทัล Azure [เป็นผู้ใช้ที่มีการเข้าถึงใบแจ้งหนี้](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **เลือกใบแจ้งหนี้**
- คลิก **ดาวน์โหลดใบแจ้งหนี้** เพื่อดูสําเนาใบแจ้งหนี้ PDF ของคุณ หากระบุว่า **ไม่พร้อมใช้งาน** ให้ดู [เหตุใดฉันจึงไม่เห็นใบแจ้งหนี้ในช่วงการเรียกเก็บเงินครั้งล่าสุด](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**รับใบแจ้งหนี้ในอีเมล (.pdf)**

- เลือกการสมัครใช้งานของคุณ [จากหน้า](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) การสมัครใช้งาน คลิก **ใบแจ้งหนี้ แล้วเลือก** ส่งอีเมลใบแจ้งหนี้ของฉัน
- คลิก **เลือก** รับ และยอมรับข้อใดข้อหนึ่ง คุณจะต้องเลือกรับการสมัครใช้งานแต่ละรายการที่คุณเป็นเจ้าของ

หมายเหตุ: ถ้าคุณไม่ได้รับอีเมลหลังจากปฏิบัติตามขั้นตอนแล้ว ตรวจสอบให้แน่ใจว่าที่อยู่อีเมลของคุณถูกต้องในการกตั้งค่า [การสื่อสารบนโปรไฟล์ของคุณ](https://account.windowsazure.com/profile)

**ดาวน์โหลดข้อมูลการใช้งานของคุณจากพอร์ทัล Azure**

- ลงชื่อเข้าใช้ศูนย์ [บัญชี Azure](https://account.windowsazure.com/Subscriptions) ในฐานะ [ผู้ดูแลระบบบัญชี](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- เลือกการสมัครใช้งานที่คุณต้องการรับข้อมูลใบแจ้งหนี้และการใช้งาน
- เลือก **ประวัติการเรียกเก็บเงิน**
- **เลือก ดูใบแจ้งยอด** ปัจจุบัน เพื่อดูค่าประมาณของค่าธรรมเนียมของคุณณ เวลาที่สร้างการประเมิน
- เลือก **ดาวน์โหลด** การใช้งาน เพื่อดาวน์โหลดข้อมูลการใช้งานรายวันเป็นไฟล์ CSV ถ้าคุณเห็นสองเวอร์ชันที่พร้อมใช้งาน ให้ดาวน์โหลดเวอร์ชัน 2

ข้อสงสัยอื่นๆ: [เยี่ยมชมเอกสารอินสแตนซ์ที่สงวนไว้](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนา**

- [ข้อมูลพื้นฐานการเรียกเก็บเงิน](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [เข้าใจวิธีการใช้ส่วนลดอินสแตนซ์แบบเหมาจ่าย](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ดาวน์โหลดหรือดูใบแจ้งหนี้การเรียกเก็บเงิน Azure และข้อมูลการใช้งานรายวันของคุณ](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [เข้าใจวิธีการใช้ส่วนลดอินสแตนซ์แบบเหมาจ่าย](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ทําความเข้าใจการใช้งานอินสแตนซ์แบบเหมาจ่ายล่วงหน้าของการสมัครใช้งาน Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [การเข้าใจการใช้งานอินสแตนซ์การสงวนสิทธิ์ในการลงทะเบียนองค์กรของคุณ](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ต้นทุนซอฟต์แวร์ Windows ไม่รวมอยู่ในอินสแตนซ์สงวน](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [อินสแตนซ์สงวนในโปรแกรม Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)