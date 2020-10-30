---
title: การเข้าถึงการสมัครใช้งาน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807724"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>ไม่สามารถลงชื่อเข้าใช้ Azure ได้เนื่องจากปัญหาเกี่ยวกับเบราว์เซอร์ (เบราว์เซอร์แฮงค์การหมุนไม่โหลดฯลฯ)

คุณอาจได้รับผลกระทบจากกระแสตก โปรดตรวจสอบเพื่อดูว่ามีการตกที่ต่อเนื่อง:[สถานะสถานภาพของ Azure](https://status.azure.com/status/history/)

โปรดออกจากระบบเซสชัน Azure ที่ใช้งานอยู่ทั้งหมด เริ่มโหมดแบบส่วนตัวหรือโหมดไม่ระบุตัวตนของเว็บเบราว์เซอร์ของคุณ

นอกจากนี้คุณยังสามารถลองรีเฟรชเบราว์เซอร์ใช้เบราว์เซอร์อื่นลบคุกกี้แคชได้ถ้าด้านบนไม่ทำงาน

เรียนรู้เพิ่มเติม: [แก้ไขปัญหาการลงชื่อเข้าใช้](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**ไม่สามารถเข้าถึงการสมัครใช้งานได้**

ใน [พอร์ทัล azure](https://portal.azure.com/)ตรวจสอบให้แน่ใจว่าได้เลือกไดเรกทอรี azure ที่ถูกต้องจากบัญชีผู้ใช้ที่ด้านบนขวา

ใน [ศูนย์บัญชี Azure](https://account.windowsazure.com/Subscriptions)ให้ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ที่ใช้เป็นผู้ดูแลระบบบัญชีผู้ใช้หรือไม่

เรียนรู้เพิ่มเติม:[แก้ไขปัญหาไม่พบการสมัคร](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)ใช้งาน

**ไม่สามารถเข้าถึงประวัติการเรียกเก็บเงินได้**

ผู้ดูแลระบบบัญชีผู้ใช้จำเป็นต้องตรวจสอบให้แน่ใจว่าผู้ใช้เข้าถึงข้อมูลการเรียกเก็บเงินจะถูกเพิ่มใน Azure Active directory เป็นผู้ใช้ที่เป็นผู้เยี่ยมชม:[เพิ่มหรือลบผู้ใช้ใหม่](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

ผู้ใช้จำเป็นต้องได้รับบทบาทผู้ดูแลระบบส่วนกลาง:[กำหนดบทบาทให้กับผู้ใช้](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

โพสต์นี้ผู้ใช้สามารถได้รับการเข้าถึงการเรียกเก็บเงินโดยใช้นโยบาย RBAC:[ให้สิทธิ์การเข้าถึงการเรียกเก็บเงิน](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนำ**

-   [ฉันไม่สามารถลงชื่อเข้าใช้เพื่อจัดการการสมัครใช้งาน Azure ของฉัน](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)