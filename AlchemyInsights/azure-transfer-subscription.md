---
title: โอนสิทธิ์ความเป็นเจ้าของการเรียกเก็บเงิน Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820629"
---
# <a name="transfer-azure-billing-ownership"></a>โอนสิทธิ์ความเป็นเจ้าของการเรียกเก็บเงิน Azure

ลงชื่อเข้าใช้พอร์ทัล [Azure](https://portal.azure.com/) ในฐานะผู้ดูแลระบบของบัญชีการเรียกเก็บเงินที่มีการสมัครใช้งานที่คุณต้องการโอน ถ้าคุณไม่แน่ใจว่าคุณเป็นผู้ดูแลระบบหรือไม่ หรือคุณต้องดูว่าใครคือใคร ให้ดู ระบุ [ผู้ดูแลระบบการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)ของบัญชี

1. ค้นหา _การจัดการต้นทุน +_ การเรียกเก็บเงิน
1. **เลือก การสมัครใช้งาน** จากบานหน้าต่างด้านซ้าย ขึ้นอยู่กับการเข้าถึง คุณอาจต้องเลือกขอบเขตการเรียกเก็บเงิน แล้วเลือก **การสมัครใช้งาน หรือ****การสมัครใช้งาน Azure**
1. เลือก **โอนความเป็นเจ้าของ** การเรียกเก็บเงิน ของการสมัครใช้งานที่คุณต้องการถ่ายโอน
1. ใส่ที่อยู่อีเมลของผู้ใช้ที่เป็นผู้ดูแลระบบการเรียกเก็บเงินของบัญชีที่จะเป็นเจ้าของใหม่การสมัครใช้งาน แล้วเลือก ส่ง **การร้องขอ** การโอน
1. ผู้ใช้จะได้รับอีเมลที่มีคําแนะนําเพื่อตรวจสอบคําขอถ่ายโอนของคุณ เมื่อต้องการอนุมัติคําขอโอน ผู้ใช้จะเลือกลิงก์ในอีเมล และปฏิบัติตามคําแนะนํา

โปรดทราบว่า ถ้าคุณถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งานของคุณไปยังบัญชีของผู้ใช้ในผู้เช่า Azure AD อื่น งานที่มอบหมายการเข้าถึงตามบทบาท [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ทั้งหมดเพื่อจัดการทรัพยากรในการสมัครใช้งานจะถูกเอาออกอย่างถาวร เฉพาะเจ้าของใหม่เท่านั้นที่จะมีสิทธิ์เข้าถึงเพื่อจัดการทรัพยากรในการสมัครใช้งาน For more information about how to change directory for a subscription, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**ผลกระทบที่สําคัญในใบแจ้งหนี้**_ ของคุณ: ถ้าคุณได้โอนสิทธิ์ความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Azure การเรียกเก็บเงินของคุณจะได้รับการให้คะแนนตามสัดส่วน คุณจะสามารถเข้าถึงใบแจ้งหนี้ตามรายการต่อไปนี้:  

1. เลือกการสมัครใช้งานของคุณ [จากหน้า](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)   การสมัครใช้งานในพอร์ทัล Azure [ในฐานะผู้ใช้ที่มีสิทธิ์](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)เข้าถึงใบแจ้งหนี้ **จากนั้นเลือก** ใบแจ้งหนี้
1. คลิก **ดาวน์โหลดใบแจ้งหนี้**   เพื่อดูสําเนาใบแจ้งหนี้ PDF ของคุณ หากระบุว่า _ไม่พร้อมใช้งาน_ ให้ดู [เหตุใดฉันจึงไม่เห็นใบแจ้งหนี้ในช่วงการเรียกเก็บเงินล่าสุด](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. คุณยังสามารถดูการใช้งานรายวันของคุณโดยการคลิกระยะเวลาการเรียกเก็บเงิน **เพื่อรับ** PDF ของใบแจ้งหนี้และสําเนาของไฟล์การใช้งานรายวันโดยละเอียดของคุณ ( CSV) หากต้องการข้อมูลเพิ่มเติม โปรดดู [รับข้อมูลใบแจ้งหนี้และการใช้](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนา**

- [โอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Azure ไปยังบัญชีอื่น](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [เกี่ยวกับการโอนสิทธิ์ความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [การโอน Visual Studio, Microsoft Partner Network (MPN) และ Pay เมื่อคุณใช้งานการสมัครใช้งาน Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [โอนย้ายความเป็นเจ้าของที่ถามบ่อย](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [แก้ไขปัญหาการโอนสิทธิ์ความเป็นเจ้าของ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
