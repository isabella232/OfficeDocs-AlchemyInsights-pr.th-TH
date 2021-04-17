---
title: ชนิดการสมัครใช้งานที่ได้รับการสนับสนุน
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
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820701"
---
# <a name="supported-subscription-types"></a>ชนิดการสมัครใช้งานที่ได้รับการสนับสนุน

โปรดตรวจสอบประเภทการสมัครใช้งานที่สนับสนุนเพื่อดําเนินการต่อ

[ชนิดการสมัครใช้งานที่ได้รับการสนับสนุน](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**ถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงิน**

พอร์ทัล Azure [ในฐานะผู้ดูแลระบบ](https://ms.portal.azure.com/) บัญชีของบัญชีการเรียกเก็บเงินที่มีการสมัครใช้งานที่คุณต้องการถ่ายโอน

- ค้นหาเกี่ยวกับ **การจัดการต้นทุน +** การเรียกเก็บเงิน **เลือก การสมัครใช้งาน** จากบานหน้าต่างด้านซ้าย ขึ้นอยู่กับการเข้าถึง คุณอาจต้องเลือกขอบเขตการเรียกเก็บเงิน แล้วเลือก **การสมัครใช้งาน หรือ****การสมัครใช้งาน Azure**
- เลือก โอนความเป็นเจ้าของการเรียกเก็บเงิน ของการสมัครใช้งานที่คุณต้องการถ่ายโอน
- ใส่ที่อยู่อีเมลของผู้ใช้ที่เป็นผู้ดูแลระบบการเรียกเก็บเงินของบัญชีที่จะเป็นเจ้าของใหม่เพื่อขอการสมัครใช้งาน แล้วเลือก ส่งการร้องขอ **การโอน**
- ผู้ใช้จะได้รับอีเมลที่มีคําแนะนําเพื่อตรวจสอบคําขอถ่ายโอนของคุณ เมื่อต้องการอนุมัติคําขอโอน ผู้ใช้จะเลือกลิงก์ในอีเมล และปฏิบัติตามคําแนะนํา

หมายเหตุ: ถ้าคุณถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งานของคุณไปยังบัญชีของผู้ใช้ในผู้เช่า Azure AD อื่น งานที่มอบหมายการเข้าถึงตามบทบาท [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ทั้งหมดเพื่อจัดการทรัพยากรในการสมัครใช้งานจะถูกเอาออกอย่างถาวร เฉพาะเจ้าของใหม่เท่านั้นที่จะมีสิทธิ์เข้าถึงเพื่อจัดการทรัพยากรในการสมัครใช้งาน For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**ถ่ายโอนความเป็นเจ้าของการสมัครใช้งาน**

บทบาทเบื้องต้นของการโอนสิทธิ์ความเป็นเจ้าของการสมัครใช้งาน (RBAC) เพื่อจัดการทรัพยากรในการสมัครใช้งานจะสูญเสียการเข้าถึง For more information about adding an existing subscription to a tenant, [see Associate or add an Azure subscription to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- การถ่ายโอนการสมัครใช้งานที่มียอดค้างอยู่จากรอบการเรียกเก็บเงินปัจจุบันจะไม่ถูกถ่ายโอนไปยังเครื่องมือการช้เงินใหม่ในบัญชีใหม่ ข้อมูลเดียวที่พร้อมใช้งานให้กับผู้ใช้ในบัญชีใหม่คือค่าใช้จ่ายของเดือนที่แล้วในการสมัครใช้งานของคุณ ส่วนที่เหลือของการใช้งานและประวัติการเรียกเก็บเงินจะไม่ถูกถ่ายโอนกับการสมัครใช้งาน
- ถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Enterprise Agreement (EA) ได้รับการสนับสนุนในพอร์ทัลข้อตกลงระดับองค์กรเท่านั้น
- Transfering a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request
- ทรัพยากรทั้งหมด เช่น เครื่องเสมือน ดิสก์ และเว็บไซต์ที่ถ่ายโอนไปยังบัญชีใหม่เสร็จสมบูรณ์ แหล่งข้อมูลต่อไปนี้อาจได้รับผลกระทบในการถ่ายโอนการสมัครใช้งานข้ามผู้เช่า:

**บริการโดเมน Azure AD**

Azure Key Vaults

- [ผู้ใช้และฐานข้อมูลที่เกี่ยวข้องกับ SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) อาจได้รับผลกระทบ โดยเฉพาะอย่างยิ่งถ้าลูกค้าใช้การรับรองความถูกต้องที่เกี่ยวข้องกับ Azure Active Directory
- **บริการแอป** ที่กําหนดค่าด้วยการรับรองความถูกต้องของ Azure Active Directory อาจได้รับผลกระทบ
- **ทีม Visual Studio** บัญชีบริการที่เชื่อมต่อกับการสมัครใช้งาน Azure อาจสูญเสียการเข้าถึงชั่วคราวเมื่อการสมัครใช้งาน Azure ที่เชื่อมต่ออยู่ถูกยกเลิก

**เอกสารที่แนะนา**

ขั้นตอนหลังจากยอมรับความเป็นเจ้าของการเรียกเก็บเงิน:

- เมื่อต้องการรักษาความเป็นเจ้าของการเรียกเก็บเงิน แต่เปลี่ยนประเภทของการสมัครใช้งาน ของคุณ ให้ดู: [สลับการสมัครใช้งาน Azure ของคุณไปยังข้อเสนออื่น](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [การโอน Visual Studio, Microsoft Partner Network (MPN) และ Pay เมื่อคุณใช้งานการสมัครใช้งาน Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [ถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [โอนย้ายความเป็นเจ้าของที่ถามบ่อย](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [แก้ไขปัญหาการโอนสิทธิ์ความเป็นเจ้าของ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)