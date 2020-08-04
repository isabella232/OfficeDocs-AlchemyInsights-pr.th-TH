---
title: ปัญหาในการใช้คอนโซลผู้ดูแลระบบ Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555880"
---
# <a name="problems-using-the-intune-admin-console"></a>ปัญหาในการใช้คอนโซลผู้ดูแลระบบ Intun

**"การเข้าถึงถูกปฏิเสธ"**

- หากคุณเป็นสมาชิกของบทบาทแบบกําหนดเองของ Intunem ให้ตรวจสอบว่ามีการกําหนดสิทธิ์การใช้งาน Intun หรือ Enterprise Mobility Suite (EMS) ให้กับบัญชีของคุณ
- ถ้าคุณกําลังใช้ตัวจัดการการตั้งค่าคอนฟิกเพื่อจัดการอุปกรณ์ ตรวจสอบคุณไม่ได้เป็นส่วนหนึ่งของคอลเลกชันผู้ใช้ Intun
- ตรวจสอบว่า คุณได้รับการกําหนดสิทธิ์การควบคุมดูแลตามบทบาทที่เหมาะสม (RBAC) ในใบบังคับบทบาท Intun
- ตรวจสอบว่ากลุ่มที่ใช้ไม่ใช่รายชื่อการแจกจ่าย Intuner inพอร์ทัล Azure สนับสนุนเฉพาะบัญชีผู้ใช้ที่อยู่ในกลุ่มความปลอดภัยของ Azure Active Directory ตรวจทานกลุ่มของคุณในพอร์ทัล Azure >กลุ่ม**Intun หรือ**  >  **Groups**ในพอร์ทัล Azure >**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**

**ผู้ใช้มีสิทธิ์มากเกินไปสําหรับบทบาท Intun**

แนะนําให้ผู้ใช้ไปที่บทบาท**Intune**  >  **Intuner Intun**  >  **My permissions**  >  **Export**

**ฉันได้เพิ่มกลุ่มขอบเขตลงในบทบาท แต่ผู้ใช้ในบทบาทนั้นยังคงเห็นผู้ใช้หรืออุปกรณ์อื่นๆ**

กลุ่มขอบเขตไม่กรองผู้ใช้หรืออุปกรณ์ กลุ่มขอบเขต:

- จํากัดผู้ที่สามารถกําหนดนโยบายหรือแอปพลิเคชันได้
- อนุญาตให้เฉพาะผู้ใช้เฉพาะรายเท่านั้นที่จะเรียกใช้งานระยะไกลบนอุปกรณ์

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่มขอบเขต ให้ดูที่[การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intun](https://docs.microsoft.com/intune/role-based-access-control)

**ฉันเพิ่มผู้ใช้ในบทบาท Intun**

นําทางไปยัง Intun>**ผู้ใช้**ในพอร์ทัล Azure และตรวจสอบว่า ผู้ใช้ไม่ได้กําหนดให้กับบทบาทต่อไปนี้ในพอร์ทัล Azure:

- ผู้ดูแลระบบส่วนกลาง
- ผู้ดูแลบริการ Intun
- ผู้ดูแล SharePoint

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intun](https://docs.microsoft.com/intune/role-based-access-control)

**ปัญหาการเข้าถึง**

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[คุณไม่สามารถลงชื่อเข้าใช้ Office 365, Azure หรือ Intun](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)