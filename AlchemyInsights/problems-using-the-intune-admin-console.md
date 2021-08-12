---
title: ปัญหาในการใช้คอนโซลผู้ดูแลระบบ Intun1
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944150"
---
# <a name="problems-using-the-intune-admin-console"></a>ปัญหาในการใช้คอนโซลผู้ดูแลระบบ Intun1

**"การเข้าถึงถูกปฏิเสธ" เมื่อนําทางพอร์ทัลผู้ดูแลระบบ Intun1**

- ถ้าคุณเป็นสมาชิกของบทบาทแบบปรับแต่งเองของ Intun1 ตรวจสอบให้แน่ใจว่าสิทธิการใช้งาน Intunอีเมล หรือ Enterprise Mobility Suite (EMS) ได้รับการมอบหมายให้กับบัญชีของคุณ
- ถ้าคุณใช้ตัวจัดการการกําหนดค่าเพื่อจัดการอุปกรณ์ ให้ตรวจสอบว่าคุณไม่ได้เป็นส่วนหนึ่งของคอลเลกชันผู้ใช้ Intun1 ใน MDM ของตัวจัดการการกําหนดค่า
- ตรวจสอบว่าคุณได้รับมอบหมายสิทธิ์การควบคุมการดูแลตามบทบาท (RBAC) ที่เหมาะสมในเบลดบทบาท Intun1
- ตรวจสอบว่ากลุ่มที่ใช้ไม่ใช่รายชื่อการแจกจ่าย Intuned ในพอร์ทัล Azure สนับสนุนเฉพาะบัญชีผู้ใช้ที่เป็นAzure Active Directoryกลุ่มความปลอดภัยเท่านั้น ตรวจสอบกลุ่มของคุณในพอร์ทัล Azure > **Intuned**  >  **Groups** หรือในพอร์ทัล Azure > **Azure Active Directory**

**ผู้ใช้มีสิทธิ์มากเกินไปในบทบาท Intun1 ที่มอบหมาย**

แนะให้ผู้ใช้ไปยังบทบาท **Intuned**  >  **Intuned**  >  **สิทธิ์**  >  **ของฉัน ส่งออก** เพื่อตรวจทานสิทธิ์ที่ให้

**ฉันได้เพิ่มกลุ่มขอบเขตลงในบทบาท แต่ผู้ใช้ในบทบาทนั้นยังคงเห็นผู้ใช้หรืออุปกรณ์อื่นๆ**

กลุ่มขอบเขตจะไม่กรองผู้ใช้หรืออุปกรณ์ออก กลุ่มขอบเขต:

- จํากัดบุคคลที่ผู้ใช้สามารถกําหนดนโยบายหรือแอปพลิเคชันให้
- อนุญาตให้ผู้ใช้ที่ระบุเท่านั้นที่จะเรียกใช้งานระยะไกลบนอุปกรณ์ได้

For more information about scope groups, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**ฉันได้เพิ่มผู้ใช้ลงในบทบาท Intun1 แต่พวกเขายังคงสามารถเข้าถึงคอนโซลผู้ดูแลระบบ Intun1 ได้อย่างเต็มที่**

นําทางไปยัง > **Intun>** ผู้ใช้ ในพอร์ทัล Azure และตรวจสอบว่าไม่ได้มอบหมายผู้ใช้ให้กับบทบาทต่อไปนี้ในพอร์ทัล Azure:

- ผู้ดูแลระบบส่วนกลาง
- ผู้ดูแลระบบบริการ Intun1
- SharePointผู้ดูแลระบบ

For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**ปัญหาการเข้าถึง**

ดูข้อมูลเพิ่มเติมได้ที่[คุณไม่สามารถลงชื่อเข้าใช้ Office 365, Azure หรือ Intuned](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)