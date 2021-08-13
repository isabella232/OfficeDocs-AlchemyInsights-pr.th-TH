---
title: ปัญหาเกี่ยวกับกลุ่มความปลอดภัย
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925760"
---
# <a name="issue-with-security-groups"></a>ปัญหาเกี่ยวกับกลุ่มความปลอดภัย

**ถ้าคุณได้รับข้อผิดพลาดเครือข่าย AADDS104**

กฎของกลุ่มความปลอดภัยของเครือข่ายที่ไม่ถูกต้องเป็นสาเหตุที่พบบ่อยที่สุดของข้อผิดพลาดเครือข่ายAzure Active Directory Domain Services (AD DS) กลุ่มความปลอดภัยของเครือข่ายของเครือข่ายเสมือนต้องอนุญาตให้เข้าถึงพอร์ตและโพรโทคอลที่เฉพาะเจาะจงได้ ถ้าพอร์ตเหล่านี้ถูกบล็อก แพลตฟอร์ม Azure ไม่สามารถตรวจสอบหรืออัปเดตโดเมนที่มีการจัดการได้ การซิงโครไนซ์ระหว่าง Azure AD และ Azure AD DS ยังได้รับผลกระทบอีกด้วย ตรวจสอบให้แน่ใจว่าคุณเปิดพอร์ตเริ่มต้นไว้เพื่อไม่ให้บริการขัดข้อง

เมื่อต้องการเข้าใจและแก้ไขปัญหาการกําหนดค่ากลุ่มความปลอดภัยของเครือข่ายที่พบทั่วไป ให้ดูที่ [เพิ่มและตรวจสอบกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)ความปลอดภัย
