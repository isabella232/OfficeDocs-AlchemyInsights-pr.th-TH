---
title: แก้ไขนโยบายตัวกรองภาษา/IP
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
ms.openlocfilehash: 25744bee6f3ed06ae67fc3c246c7d64fce9994bb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320544"
---
# <a name="fix-languageip-filter-policy"></a>แก้ไขนโยบายตัวกรองภาษา/IP

นโยบายป้องกันสแปมนโยบายใดนโยบายหนึ่งของคุณที่ได้รับผลกระทบจากข้อความนี้ เมื่อต้องการตรวจสอบนโยบาย ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ในMicrosoft 365 Defenderที่ <https://security.microsoft.com/> ให้ไปที่ นโยบาย **&การ**& \> **นโยบาย** \> **ภัยคุกคาม** ทางอีเมล \> **ในส่วน** นโยบาย

   เมื่อต้องการไปที่หน้า **นโยบายป้องกันสแปม** <https://security.microsoft.com/antispam> โดยตรง ให้ใช้

2. บนหน้า **นโยบายป้องกันสแปม** ให้เลือกนโยบายโดยการคลิกที่ชื่อของนโยบาย (ชนิดคือนโยบายการป้องกัน **สแปม** แบบเองหรือ ชื่อ คือ นโยบายขาเข้าของการป้องกันสแปม **(ค่าเริ่มต้น)**)
3. ในปลิวรายละเอียดที่ปรากฏขึ้น ให้เลือก **แก้ไขค่าเกณฑ์และคุณสมบัติสแปม** ในค่าเกณฑ์ **&อีเมลกลุ่มใหญ่ ในส่วน คุณสมบัติ** สแปม
4. ในส่วน **เครื่องหมายเป็นสแปม** ให้ตรวจทานการตั้งค่า **ประกอบด้วยภาษา** ที่ระบุ **และ จากประเทศ** เหล่านี้

For more information, see [Configure anti-spam policies in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
