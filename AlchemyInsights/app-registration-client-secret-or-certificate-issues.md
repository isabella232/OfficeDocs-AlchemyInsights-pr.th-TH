---
title: ปัญหาข้อมูลลับหรือใบรับรองของไคลเอ็นต์การลงทะเบียนแอป
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405330"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>ปัญหาความลับหรือใบรับรองของไคลเอ็นต์การลงทะเบียนแอป

ไคลเอ็นต์แอปพลิเคชันหมดอายุลงหรือไม่

ไม่ว่าจะสร้างแอปพลิเคชันที่ลงทะเบียนไว้อย่างไร ไม่ว่าจะผ่านขั้นตอนการลงทะเบียนมาตรฐานในพอร์ทัลการลงทะเบียนแอป หรือถ้าหลักของบริการถูกสร้างขึ้นในผู้เช่าของคุณโดยใช้ความยินยอมของแอปพลิเคชัน ข้อมูลลับไคลเอ็นต์ใหม่จะถูกสร้างขึ้นก่อนที่จะหมดอายุของรหัสแอปพลิเคชันปัจจุบันและถูกอัปเดตในรหัสแอปพลิเคชันที่เกี่ยวข้อง ระยะเวลาที่ใช้ได้สูงสุดคือ 2 ปี ในฐานะที่เป็นตัวเตือน ค่าลับต้องถูกบันทึกเนื่องจากจะไม่สามารถมองเห็นได้อีกต่อไปหลังจากออกจากหน้าการลงทะเบียนแอปในพอร์ทัล ดูข้อมูลเริ่มต้นใช้งานด่วน:[ลงทะเบียนแอปในแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)และหลักปฏิบัติ[ที่ดีที่สุดเกี่ยวกับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [สร้างแอป Azure AD &หลักของบริการในพอร์ทัล - แพลตฟอร์มข้อมูลเฉพาะตัวของ](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)Microsoft
