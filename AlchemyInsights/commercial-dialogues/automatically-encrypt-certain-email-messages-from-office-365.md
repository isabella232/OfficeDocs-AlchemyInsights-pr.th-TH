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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749454"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>เข้ารหัสลับบางข้อความอีเมลจาก Office 365 โดยอัตโนมัติ

1. จากศูนย์ [การจัดการ Exchange](https://outlook.office365.com/ecp/)ให้เลือก **ล>จดหมายตาม** กฎ 
2. คลิกไอคอน **ใหม่ (+)** แล้วคลิก ใช้การเข้ารหัสลับข้อความและการป้องกันสิทธิ์ของ **Office 365 กับ** ข้อความ
3. ในชื่อ ให้ใส่ชื่อของกฎ เช่น *เข้ารหัสลับข้อความ* ทั้งหมด
4. ใน **ใช้กฎนี้ ถ้า** เลือก **[ใช้กับข้อความทั้งหมด]** 
5. ถัดจากเขตข้อมูล **Do the following** ให้คลิก **เลือกหนึ่ง** รายการ 
6. ในเมนูดรอปดาวน์ของเทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง (ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ แต่คุณสามารถเพิ่มได้)
7. เลือกกล่องกา **เครื่องหมาย ตรวจสอบกฎนี้ด้วย** ระดับความรุนแรง แล้วเลือกระดับที่ต้องการ ถ้าบริษัทของคุณมีข้อผูกมัดสัญญาที่จะส่งอีเมลทั้งหมดที่เข้ารหัสลับ ฉันขอแนะนนะให้ตั้งค่า **ระดับเป็น** สูง
8. ภายใต้ **เลือกตัวแบบของกฎ** นี้ **ให้คลิก** บังคับใช้ 
9. เลือกตัวเลือกใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างด้วยการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)
10. คลิก **บันทึก**

> [!IMPORTANT]
> คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ

For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

