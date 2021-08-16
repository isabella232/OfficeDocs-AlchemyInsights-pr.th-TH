---
title: เข้ารหัสลับOffice 365ที่ส่งไปยังโดเมนบางโดเมนโดยอัตโนมัติ
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082205"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>เข้ารหัสลับOffice 365ที่ส่งไปยังโดเมนบางโดเมนโดยอัตโนมัติ

1. จากศูนย์ [Exchangeจดหมาย](https://outlook.office365.com/ecp/)เลือก **ล>จดหมาย ตาม** กฎ 
2. คลิก **ไอคอน ใหม่ (+)** แล้วคลิก การเข้ารหัสลับข้อความของ Office 365 **การป้องกันสิทธิ์กับ** ข้อความ
3. ในชื่อ ให้ใส่ชื่อกฎ เช่น เข้ารหัสลับ *ข้อความที่ส่งไปยัง contoso.com*
4. ใน **ใช้กฎนี้** ถ้า **เลือก >โดเมน** คือ 
5. ใส่ชื่อของโดเมน เช่น **contoso.com**
6. คลิก **ไอคอน เพิ่ม (+)** **แล้วคลิก** ตกลง
7. ถัดจากเขตข้อมูล **Do the following** ให้คลิก **Select one** 
8. ในเมนูดรอปดาวน์เทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง (ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ แต่คุณสามารถเพิ่มได้!)
9. เลือกตัวเลือกเพิ่มเติมใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างที่มีการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)
10. คลิก **บันทึก**

> [!IMPORTANT]
> คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ

For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)