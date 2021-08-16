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
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072179"
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
- ถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงินEnterprise Agreementการสมัครใช้งาน (EA) ได้รับการสนับสนุนในพอร์ทัล Enterprise Agreementเท่านั้น
- Transfering a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request
- ทรัพยากรทั้งหมด เช่น เครื่องเสมือน ดิสก์ และเว็บไซต์ที่ถ่ายโอนไปยังบัญชีใหม่เสร็จสมบูรณ์ แหล่งข้อมูลต่อไปนี้อาจได้รับผลกระทบในการถ่ายโอนการสมัครใช้งานข้ามผู้เช่า:

**บริการโดเมน Azure AD**

Azure Key Vaults

- [SQLและฐานข้อมูลที่เกี่ยวข้อง](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)อาจได้รับผลกระทบ โดยเฉพาะอย่างยิ่ง ถ้าลูกค้าใช้การรับรองความถูกต้องAzure Active Directoryที่สัมพันธ์กัน
- **บริการแอป** ที่กําหนดค่าAzure Active Directoryการรับรองความถูกต้องอาจได้รับผลกระทบ
- **Visual Studioทีม** บัญชีบริการที่เชื่อมต่อกับการสมัครใช้งาน Azure อาจสูญเสียการเข้าถึงชั่วคราวเมื่อการสมัครใช้งาน Azure ที่เชื่อมต่ออยู่ถูกยกเลิก

**เอกสารที่แนะนา**

ขั้นตอนหลังจากยอมรับความเป็นเจ้าของการเรียกเก็บเงิน:

- เมื่อต้องการรักษาความเป็นเจ้าของการเรียกเก็บเงิน แต่เปลี่ยนประเภทของการสมัครใช้งาน ของคุณ ให้ดู: [สลับการสมัครใช้งาน Azure ของคุณไปยังข้อเสนออื่น](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [การโอนVisual Studio, Microsoft Partner Network (MPN) และ Pay as you go Dev/Test subscriptions](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [ถ่ายโอนความเป็นเจ้าของการเรียกเก็บเงินEnterprise Agreementการสมัครใช้งาน (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [โอนย้ายความเป็นเจ้าของที่ถามบ่อย](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [แก้ไขปัญหาการโอนสิทธิ์ความเป็นเจ้าของ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)