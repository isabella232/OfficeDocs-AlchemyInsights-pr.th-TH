---
title: โอนสิทธิ์การเรียกเก็บเงิน Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736897"
---
# <a name="transfer-azure-billing-ownership"></a>โอนสิทธิ์การเรียกเก็บเงิน Azure

ลงชื่อเข้าใช้ [พอร์ทัล Azure](https://portal.azure.com/) ในฐานะผู้ดูแลระบบของบัญชีผู้ใช้การเรียกเก็บเงินที่มีการสมัครใช้งานที่คุณต้องการโอนย้าย ถ้าคุณไม่แน่ใจว่าคุณเป็นผู้ดูแลระบบหรือไม่หรือถ้าคุณต้องการกำหนดผู้ใช้ให้ดูที่[กำหนดผู้ดูแลระบบการเรียกเก็บเงินของบัญชีผู้ใช้](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)

1. ค้นหา _การจัดการต้นทุน + การเรียกเก็บเงิน_
1. เลือกการ **สมัคร** ใช้งานจากบานหน้าต่างด้านซ้าย คุณอาจจำเป็นต้องเลือกขอบเขตการเรียกเก็บเงินจากนั้นการ **สมัคร** ใช้งานหรือการสมัครใช้งาน **Azure** ทั้งนี้ขึ้นอยู่กับการเข้าถึง
1. เลือก **โอนความเป็นเจ้าของการเรียกเก็บเงิน** สำหรับการสมัครใช้งานที่คุณต้องการโอนย้าย
1. ใส่ที่อยู่อีเมลของผู้ใช้ที่เป็นผู้ดูแลการเรียกเก็บเงินของบัญชีผู้ใช้ที่จะเป็นเจ้าของใหม่สำหรับการสมัครใช้งานแล้วเลือก **ส่งคำขอการโอนย้าย**
1. ผู้ใช้ได้รับอีเมลที่มีคำแนะนำในการตรวจสอบคำขอการโอนย้ายของคุณ เมื่อต้องการอนุมัติคำขอการโอนย้ายผู้ใช้จะเลือกลิงก์ในอีเมลและตามคำแนะนำ

โปรดทราบว่าถ้าคุณโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งานของคุณไปยังบัญชีผู้ใช้ของคุณในผู้เช่า Azure AD อื่น [ตัวควบคุมการเข้าถึงตามบทบาททั้งหมด (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ที่มอบหมายเพื่อจัดการทรัพยากรในการสมัครใช้งานจะถูกเอาออกอย่างถาวร เฉพาะเจ้าของใหม่เท่านั้นที่จะมีสิทธิ์เข้าถึงเพื่อจัดการทรัพยากรในการสมัครใช้งาน สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเปลี่ยนไดเรกทอรีสำหรับการสมัครใช้งานให้ดูที่การ[โอนการสมัครใช้งานไปยังผู้ใช้ในผู้เช่า AZURE AD รายอื่น](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

_**ผลกระทบที่สำคัญบนใบแจ้งหนี้ของคุณ**_: ถ้าคุณได้โอนสิทธิ์การเรียกเก็บเงินสำหรับการสมัครใช้งาน Azure การเรียกเก็บเงินของคุณจะได้รับการจัดอันดับเป็น pro คุณจะสามารถเข้าถึงใบแจ้งหนี้ได้ดังต่อไปนี้:  

1. เลือกการสมัครใช้งานของคุณจาก [หน้าการสมัคร](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)ใช้   งานในพอร์ทัล Azure เป็น [ผู้ใช้ที่มีสิทธิ์เข้าถึงใบแจ้งหนี้](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)จากนั้นเลือก **ใบแจ้งหนี้**
1. คลิก **ดาวน์โหลดใบแจ้งหนี้**   เพื่อดูสำเนาใบแจ้งหนี้ PDF ของคุณ ถ้า _ไม่มี_ ให้ดู [ที่ทำไมฉันจึงไม่เห็นใบแจ้งหนี้สำหรับช่วงเวลาการเรียกเก็บเงินล่าสุด](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. นอกจากนี้คุณยังสามารถดูการใช้งานประจำวันของคุณได้โดยการคลิกที่ **ช่วงเวลาการเรียกเก็บเงิน** เพื่อรับ PDF ของใบแจ้งหนี้ของคุณและสำเนาของไฟล์การใช้งานประจำวันที่มีรายละเอียดของคุณ ( CSV) สำหรับข้อมูลเพิ่มเติมให้ดูที่ [รับใบแจ้งหนี้และข้อมูลการใช้งาน](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนำ**

- [โอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Azure ไปยังบัญชีผู้ใช้อื่น](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [เกี่ยวกับการโอนความเป็นเจ้าของการเรียกเก็บเงินสำหรับการสมัครใช้งาน Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [การถ่ายโอน Visual Studio, Microsoft Partner Network (MPN) และชำระเงินตามที่คุณไปยังการสมัครใช้งาน Dev/ทดสอบ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [คำถามที่ถามบ่อยเกี่ยวกับการโอนสิทธิ์](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [การแก้ไขปัญหาการโอนความเป็นเจ้าของ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
