---
title: เข้ารหัสลับบางข้อความอีเมลจาก Office 365 โดยอัตโนมัติ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988854"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>เข้ารหัสลับบางข้อความอีเมลจาก Office 365 โดยอัตโนมัติ

1. จากศูนย์ [Exchangeจดหมาย](https://outlook.office365.com/ecp/)เลือก **ล>จดหมาย ตาม** กฎ 
2. คลิก **ไอคอน ใหม่ (+)** แล้วคลิก การเข้ารหัสลับข้อความของ Office 365 **การป้องกันสิทธิ์กับ** ข้อความ
3. **ใน** ชื่อ ให้ใส่ชื่อของกฎ เช่น *เข้ารหัสลับข้อความ* ทั้งหมด
4. ใน **ใช้กฎนี้ถ้า** เลือก **[ใช้กับข้อความทั้งหมด]** 
5. ถัดจากเขตข้อมูล **Do the following** ให้คลิก **Select one** 
6. ในเมนูดรอปดาวน์เทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง (ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ แต่คุณสามารถเพิ่มได้!)
7. เลือกกล่องกา **เครื่องหมาย ตรวจสอบกฎนี้ด้วย** ระดับความรุนแรง แล้วเลือกระดับที่ต้องการ ถ้าบริษัทของคุณมีข้อผูกมัดสัญญาที่จะส่งอีเมลทั้งหมดที่เข้ารหัสลับ ฉันแนะนนะให้ตั้งค่า **ระดับเป็น** สูง
8. **ภายใต้ เลือกตัวแบบของกฎ** นี้ **ให้คลิก** บังคับใช้ 
9. เลือกตัวเลือกเพิ่มเติมใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างที่มีการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)
10. คลิก **บันทึก**

> [!IMPORTANT]
> คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ

For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

