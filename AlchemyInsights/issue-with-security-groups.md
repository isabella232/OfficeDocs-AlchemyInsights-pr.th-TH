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
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177635"
---
# <a name="issue-with-security-groups"></a>ปัญหาเกี่ยวกับกลุ่มความปลอดภัย

**ถ้าคุณได้รับข้อผิดพลาดเครือข่าย AADDS104**

กฎของกลุ่มความปลอดภัยของเครือข่ายไม่ถูกต้องเป็นสาเหตุที่พบบ่อยที่สุดของข้อผิดพลาดเครือข่ายของ Azure Active Directory Domain Services (AD DS) กลุ่มความปลอดภัยของเครือข่ายของเครือข่ายเสมือนต้องอนุญาตให้เข้าถึงพอร์ตและโพรโทคอลเฉพาะได้ ถ้าพอร์ตเหล่านี้ถูกบล็อก แพลตฟอร์ม Azure ไม่สามารถตรวจสอบหรืออัปเดตโดเมนที่มีการจัดการได้ การซิงโครไนซ์ระหว่าง Azure AD และ Azure AD DS ยังได้รับผลกระทบอีกด้วย ตรวจสอบให้แน่ใจว่าคุณเปิดพอร์ตเริ่มต้นไว้เพื่อไม่ให้บริการขัดข้อง

เมื่อต้องการเข้าใจและแก้ไขปัญหาการกําหนดค่ากลุ่มความปลอดภัยของเครือข่ายที่พบทั่วไป ให้ดูที่ [เพิ่มและตรวจสอบกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)ความปลอดภัย
