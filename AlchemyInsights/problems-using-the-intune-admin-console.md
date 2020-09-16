---
title: ปัญหาในการใช้คอนโซลผู้ดูแลระบบของ Intune
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
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728306"
---
# <a name="problems-using-the-intune-admin-console"></a>ปัญหาในการใช้คอนโซลผู้ดูแลระบบของ Intune

**"การเข้าถึงถูกปฏิเสธ" เมื่อนำทางพอร์ทัลผู้ดูแลระบบของ Intune**

- ถ้าคุณเป็นสมาชิกของบทบาทแบบกำหนดเองของ Intune ให้ตรวจสอบให้แน่ใจว่ามีการกำหนดสิทธิ์การใช้งาน Intune หรือองค์กรการเคลื่อนไหวของ Intune (EMS) ให้กับบัญชีผู้ใช้ของคุณ
- ถ้าคุณกำลังใช้ตัวจัดการการกำหนดค่าเพื่อจัดการอุปกรณ์ให้ตรวจสอบว่าคุณไม่ได้เป็นส่วนหนึ่งของคอลเลกชันของผู้ใช้ Intune สำหรับตัวจัดการการกำหนดค่า MDM
- ตรวจสอบว่าคุณได้รับสิทธิ์ที่เหมาะสมตามบทบาทการจัดการการดูแลระบบ (RBAC) ในใบมีดบทบาท Intune
- การตรวจสอบความถูกต้องของกลุ่มที่ใช้ไม่ใช่รายชื่อการแจกจ่าย Intune ในพอร์ทัล Azure สนับสนุนเฉพาะบัญชีผู้ใช้ที่เป็นสมาชิกของกลุ่มความปลอดภัยของ Azure Active directory เท่านั้น ตรวจทานกลุ่มของคุณในกลุ่มของ azure portal > **Intune**  >  **Groups**หรือใน azure portal > **azure active directory**

**ผู้ใช้มีสิทธิ์มากเกินไปสำหรับบทบาท Intune ที่ได้รับมอบหมาย**

แนะนำให้ผู้ใช้ไปที่บทบาท**intune**intune  >  **Intune roles**  >  **ของฉัน**  >  การ**ส่งออก**สิทธิ์ของฉันเพื่อตรวจทานสิทธิ์ที่ได้รับอนุญาต

**ฉันเพิ่มกลุ่มขอบเขตให้กับบทบาทแต่ผู้ใช้ในบทบาทนั้นยังคงเห็นผู้ใช้หรืออุปกรณ์อื่นๆ**

กลุ่มขอบเขตไม่กรองผู้ใช้หรืออุปกรณ์ กลุ่มขอบเขต:

- จำกัดผู้ใช้ที่สามารถกำหนดนโยบายหรือแอปพลิเคชันให้กับผู้ใช้ได้
- อนุญาตเฉพาะผู้ใช้ที่เฉพาะเจาะจงในการเรียกใช้งานระยะไกลบนอุปกรณ์

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่มขอบเขตให้ดู[ที่การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control)

**ฉันเพิ่มผู้ใช้ลงในบทบาทของ Intune แต่พวกเขายังมีสิทธิ์การเข้าถึงคอนโซลผู้ดูแลระบบ Intune แบบเต็ม**

นำทางไปยัง Intune > **ผู้ใช้** ในพอร์ทัล azure และตรวจสอบว่าผู้ใช้ไม่ได้รับมอบหมายให้กับบทบาทใดๆต่อไปนี้ในพอร์ทัล azure:

- ผู้ดูแลระบบส่วนกลาง
- ผู้ดูแลระบบบริการ Intune
- ผู้ดูแลระบบ SharePoint

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control)

**ปัญหาในการเข้าถึง**

สำหรับข้อมูลเพิ่มเติมให้ดู [ที่คุณไม่สามารถลงชื่อเข้าใช้ Office ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)ได้