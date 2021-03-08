---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527746"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ

ต่อไปนี้เป็นวิธีการตั้งค่านโยบายเพื่อย้ายอีเมลเก่าของผู้ใช้ไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ:

1. Go to [**security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data  >  **governance**  >  **Archive** to verify an archive mailbox has been enabled for the user. ถ้ายังไม่ได้เปิด ให้คลิก **เปิดใช้งาน** แล้วคลิก **ใช่** ในกล่องคําเตือน
2. ไปที่ศูนย์ [**การจัดการ Exchange >การจัดการการปฏิบัติตาม>แท็กการเก็บข้อมูล**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. เลือกไอคอน + แล้วเลือก **ใช้กับกล่องจดหมายทั้งหมด** โดยอัตโนมัติ
4. กําหนดชื่อให้กับแท็กการเก็บข้อมูล แล้วเลือก **ย้ายไปยังเก็บถาวร** ในช่วงเวลาการเก็บข้อมูล ให้ใส่เวลาที่คุณต้องการ เช่น 90 วัน คลิก **บันทึก**
5. ตอนนี้ให้สร้างนโยบายการเก็บข้อมูล **โดยเลือก** นโยบายการเก็บข้อมูล เลือกไอคอนเพื่อเพิ่มนโยบายใหม่
6. กําหนดชื่อให้กับนโยบายการเก็บข้อมูล แล้วคลิกและเลื่อนเพื่อค้นหาและเพิ่มแท็กการเก็บข้อมูลที่คุณเพิ่งสร้างขึ้น คลิก **บันทึก**
7. สุดท้าย ให้ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมายของผู้ใช้: ยังคงอยู่ในศูนย์การจัดการ Exchange ให้ไปที่  >  **กล่องจดหมาย** ผู้รับ เลือกผู้ใช้ทั้งหมดที่คุณต้องการปรับใช้นโยบาย แล้วเลือก **แก้ไข** (ไอคอนรูปดินสอ)
8. ในกล่องโต้ตอบ ให้คลิกฟีเจอร์ **ของ** กล่องจดหมาย ภายใต้ **นโยบายการเก็บ** ข้อมูล ให้ใช้นโยบายที่คุณเพิ่ง>**บันทึก**
9. For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
