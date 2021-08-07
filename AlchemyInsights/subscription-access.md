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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999259"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>ไม่สามารถลงชื่อเข้าใช้ Azure ได้เนื่องจากปัญหาเกี่ยวกับเบราว์เซอร์ (เบราว์เซอร์ค้าง ไม่หมุน ไม่โหลด และอื่นๆ)

คุณอาจได้รับผลกระทบจากการไม่อยู่ โปรดตรวจสอบเพื่อดูว่ามีสถานะไม่อยู่หรือไม่:[สถานะ Azure Health](https://status.azure.com/status/history/)

โปรดออกจากระบบของเซสชัน Azure ที่ใช้งานอยู่ทั้งหมด เริ่มโหมดแบบส่วนตัวหรือไม่ระบุตัวตนของเว็บเบราว์เซอร์ของคุณ

You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.

เรียนรู้เพิ่มเติม [: แก้ไขปัญหาการลงชื่อเข้าใช้](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**ไม่สามารถเข้าถึงการสมัครใช้งาน**

ใน [พอร์ทัล Azure](https://portal.azure.com/)ตรวจสอบให้แน่ใจว่าเลือกไดเรกทอรี Azure ที่ถูกต้องจากบัญชีที่ด้านบนขวา

ใน [ศูนย์บัญชี Azure](https://account.windowsazure.com/Subscriptions)ตรวจสอบให้แน่ใจว่าบัญชีที่ใช้คือผู้ดูแลระบบบัญชีหรือไม่

เรียนรู้เพิ่มเติม: [ไม่พบการแก้ไขปัญหาการสมัครใช้งาน](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**ไม่สามารถเข้าถึงประวัติการเรียกเก็บเงินได้**

ผู้ดูแลระบบบัญชีต้องตรวจสอบให้แน่ใจว่าผู้ใช้ที่เข้าถึงข้อมูลการเรียกเก็บเงินจะถูกเพิ่มใน Azure Active Directory เป็นผู้ใช้ที่เป็นแขก: [เพิ่มหรือลบผู้ใช้](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)ใหม่

จากนั้นผู้ใช้ต้องได้รับบทบาทผู้ดูแลระบบส่วนกลาง: [กําหนดบทบาทให้กับ](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)ผู้ใช้

โพสต์นี้ ผู้ใช้สามารถให้สิทธิ์การเข้าถึงการเรียกเก็บเงินโดยใช้นโยบาย RBAC:[ให้สิทธิ์การเข้าถึงการเรียกเก็บเงิน](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**เอกสารที่แนะนา**

-   [ฉันไม่สามารถลงชื่อเข้าใช้เพื่อจัดการการสมัครใช้งาน Azure ได้](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)