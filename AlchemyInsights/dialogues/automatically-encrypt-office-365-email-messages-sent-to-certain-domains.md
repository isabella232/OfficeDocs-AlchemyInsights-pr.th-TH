---
title: เข้ารหัสลับข้อความอีเมล Office 365 ที่ถูกส่งไปยังบางโดเมนโดยอัตโนมัติ
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527601"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>เข้ารหัสลับข้อความอีเมล Office 365 ที่ถูกส่งไปยังบางโดเมนโดยอัตโนมัติ

1. จากศูนย์ [การจัดการ Exchange](https://outlook.office365.com/ecp/)ให้เลือก **ล>จดหมายตาม** กฎ 
2. คลิกไอคอน **ใหม่ (+)** แล้วคลิก ใช้การเข้ารหัสลับข้อความและการป้องกันสิทธิ์ของ **Office 365 กับ** ข้อความ
3. ในชื่อ ให้ใส่ชื่อของกฎ เช่น เข้ารหัสข้อความที่ *ส่งไปยังcontoso.com*
4. ใน **ปรับใช้กฎนี้** ถ้า เลือก **>โดเมนคือ** 
5. ใส่ชื่อของโดเมน เช่น contoso.com 
6. คลิก **ไอคอน เพิ่ม (+)** **แล้วคลิก** ตกลง
7. ถัดจากเขตข้อมูล **Do the following** ให้คลิก **เลือกหนึ่ง** รายการ 
8. ในเมนูดรอปดาวน์ของเทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง (ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ แต่คุณสามารถเพิ่มได้)
9. เลือกตัวเลือกใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างด้วยการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)
10. คลิก **บันทึก**

> [!IMPORTANT]
> คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ

For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)