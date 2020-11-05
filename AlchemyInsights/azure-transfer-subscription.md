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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922172"
---
# <a name="transfer-azure-billing-ownership"></a>โอนสิทธิ์การเรียกเก็บเงิน Azure

ลงชื่อเข้าใช้ [พอร์ทัล Azure](https://portal.azure.com/) ในฐานะผู้ดูแลระบบของบัญชีผู้ใช้การเรียกเก็บเงินที่มีการสมัครใช้งานที่คุณต้องการโอนย้าย ถ้าคุณไม่แน่ใจว่าคุณเป็นผู้ดูแลระบบหรือไม่หรือถ้าคุณต้องการกำหนดใครให้ดูที่[กำหนดผู้ดูแลการเรียกเก็บเงินของบัญชีผู้ใช้](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)

- ค้นหา **การจัดการต้นทุน + การเรียกเก็บเงิน**
- เลือกการ **สมัคร** ใช้งานจากบานหน้าต่างด้านซ้าย คุณอาจจำเป็นต้องเลือกขอบเขตการเรียกเก็บเงินจากนั้นการ **สมัคร** ใช้งานหรือการสมัครใช้งาน **Azure** ทั้งนี้ขึ้นอยู่กับการเข้าถึง
- เลือก **โอนความเป็นเจ้าของการเรียกเก็บเงิน** สำหรับการสมัครใช้งานที่คุณต้องการโอนย้าย
- ใส่ที่อยู่อีเมลของผู้ใช้ที่เป็นผู้ดูแลการเรียกเก็บเงินของบัญชีผู้ใช้ที่จะเป็นเจ้าของใหม่สำหรับการสมัครใช้งานแล้วเลือก **ส่งคำขอการโอนย้าย**
- ผู้ใช้ได้รับอีเมลที่มีคำแนะนำในการตรวจสอบคำขอการโอนย้ายของคุณ เมื่อต้องการอนุมัติคำขอการโอนย้ายผู้ใช้จะเลือกลิงก์ในอีเมลและตามคำแนะนำ

**หมายเหตุ** : ถ้าคุณโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งานของคุณไปยังบัญชีผู้ใช้ของคุณในผู้เช่า Azure AD อื่นการมอบหมายการ [ควบคุมการเข้าถึงตามบทบาท (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)ทั้งหมดเพื่อจัดการทรัพยากรในการสมัครใช้งานจะถูกเอาออกอย่างถาวร เฉพาะเจ้าของใหม่เท่านั้นที่จะมีสิทธิ์เข้าถึงเพื่อจัดการทรัพยากรในการสมัครใช้งาน สำหรับข้อมูลเพิ่มเติมให้ดูที่[การโอนการสมัครใช้งานไปยังผู้ใช้ในผู้เช่า AZURE AD รายอื่น](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนำ**

- [โอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Azure ไปยังบัญชีผู้ใช้อื่น](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [เกี่ยวกับการโอนความเป็นเจ้าของการเรียกเก็บเงินสำหรับการสมัครใช้งาน Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [การถ่ายโอน Visual Studio, Microsoft Partner Network (MPN) และชำระเงินตามที่คุณไปยังการสมัครใช้งาน Dev/ทดสอบ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [คำถามที่ถามบ่อยเกี่ยวกับการโอนสิทธิ์](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [การแก้ไขปัญหาการโอนความเป็นเจ้าของ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
