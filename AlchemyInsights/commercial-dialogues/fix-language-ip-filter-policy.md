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
ms.openlocfilehash: 16aa12120034e1f848e62bab151d8e30b251a29e5727f085300d74ca7b49ca52
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896174"
---
# <a name="fix-languageip-filter-policy"></a>แก้ไขนโยบายตัวกรองภาษา/IP

นโยบายป้องกันสแปมนโยบายใดนโยบายหนึ่งของคุณที่ได้รับผลกระทบจากข้อความนี้ เมื่อต้องการตรวจสอบนโยบาย ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ในMicrosoft 365 Defenderอีเมลที่ <https://security.microsoft.com/> ไปที่ นโยบาย&การ& \> **ร่วมกัน** \> **ทางอีเมล** \> หรือ นโยบายภัยคุกคาม ในส่วน นโยบาย

   เมื่อต้องการไปที่หน้า **นโยบายป้องกันสแปม** <https://security.microsoft.com/antispam> โดยตรง ให้ใช้

2. บนหน้า **นโยบายป้องกันสแปม** ให้เลือกนโยบายโดยการคลิกที่ชื่อของนโยบาย (ชนิดคือนโยบายการป้องกัน **สแปม** แบบเองหรือ ชื่อ คือ นโยบายขาเข้าของการป้องกันสแปม **(ค่าเริ่มต้น)**)
3. ในรายละเอียดที่ปรากฏขึ้น ให้เลือก แก้ไข **ค่าเกณฑ์และคุณสมบัติสแปม** ในส่วน ค่าเกณฑ์ **อีเมล&สแปม**
4. ในส่วน **เครื่องหมายเป็นสแปม** ให้ตรวจทานการตั้งค่า **ประกอบด้วยภาษา** ที่ระบุ **และ จากประเทศ** เหล่านี้

For more information, see [Configure anti-spam policies in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
