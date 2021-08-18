---
title: แก้ไขนโยบายผู้เช่า (การแทนที่การปฏิบัติการ)
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
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326816"
---
# <a name="fix-tenant-policy-action-override"></a>แก้ไขนโยบายผู้เช่า (การแทนที่การปฏิบัติการ)

นโยบายป้องกันสแปมนโยบายใดนโยบายหนึ่งของคุณที่ได้รับผลกระทบจากข้อความนี้ เมื่อต้องการตรวจสอบนโยบาย ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ในMicrosoft 365 Defenderที่ <https://security.microsoft.com/> ให้ไปที่ นโยบาย **&การ**& \> **นโยบาย** \> **ภัยคุกคาม** ทางอีเมล \> **ในส่วน** นโยบาย

   เมื่อต้องการไปที่หน้า **นโยบายป้องกันสแปม** <https://security.microsoft.com/antispam> โดยตรง ให้ใช้

2. บนหน้า **นโยบายป้องกันสแปม** ให้เลือกนโยบายโดยการคลิกที่ชื่อของนโยบาย (ชนิดคือนโยบายการป้องกัน **สแปม** แบบเองหรือ ชื่อ คือ นโยบายขาเข้าของการป้องกันสแปม **(ค่าเริ่มต้น)**)
3. ในเส้นปลิวรายละเอียดที่ปรากฏขึ้น ให้เลือก **แก้ไขการแอคชัน** ในส่วน **การแอคชัน**
4. ในส่วน **การแอคชัน** ของข้อความ ให้ตรวจทานผลของสแปมความเชื่อมั่นสูง สแปม ฟิชชิ่ง และฟิชชิ่งที่มีความเชื่อมั่นสูง เพื่อดูว่าได้เลือกค่าใดๆ ต่อไปนี้ไว้
   - **เพิ่มส่วนหัว X**
   - **บรรทัดเรื่องที่ขึ้นหน้าด้วยข้อความ**
   - **เปลี่ยนเส้นทางข้อความไปยังที่อยู่อีเมล**
   - **ลบข้อความ**
   - **ไม่มีการแอคชัน**

   อาจเป็นไปได้ว่าการตั้งค่ามาตรฐาน **ที่ปรับใช้** กับExchange Online Protectionทั้งหมดมีผลต่อข้อความ

For more information, see [Configure anti-spam policies in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
