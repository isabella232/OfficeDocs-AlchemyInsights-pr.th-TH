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
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318867"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>เข้ารหัสลับOffice 365ที่ส่งไปยังโดเมนบางโดเมนโดยอัตโนมัติ

1. จากศูนย์ [Exchangeจดหมาย](https://outlook.office365.com/ecp/)เลือก **ล>จดหมาย ตาม** กฎ 
2. คลิก **ไอคอน ใหม่ (+)** แล้วคลิก การเข้ารหัสลับข้อความของ Office 365 **การป้องกันสิทธิ์กับ** ข้อความ
3. ในชื่อ ให้ใส่ชื่อของกฎ เช่น เข้ารหัสลับ *ข้อความที่ส่งไปยัง contoso.com*
4. ใน **ใช้กฎนี้** ถ้า **เลือก >โดเมน** คือ 
5. ใส่ชื่อของโดเมน เช่น **contoso.com**
6. คลิก **ไอคอน เพิ่ม (+)** **แล้วคลิก** ตกลง
7. ถัดจากเขตข้อมูล **Do the following** ให้คลิก **Select one** 
8. ในเมนูดรอปดาวน์เทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง (ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ แต่คุณสามารถเพิ่มได้!)
9. เลือกตัวเลือกเพิ่มเติมใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ ซึ่งหลายตัวเลือกสามารถเหลือไว้พร้อมกับการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)
10. คลิก **บันทึก**

**สิ่ง** สําคัญ: คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ

For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)