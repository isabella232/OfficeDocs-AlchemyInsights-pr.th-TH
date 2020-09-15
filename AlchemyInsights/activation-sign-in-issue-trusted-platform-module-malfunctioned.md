---
title: การเปิดใช้งาน/ปัญหาในการลงชื่อเข้าใช้-โมดูลของ platform ที่เชื่อถือได้ปกติ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 13e6fcd18047e511452f0180dc2e4677466d4db3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697540"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>การแก้ไขแอป Microsoft ๓๖๕ "โมดูลของ Platform ที่เชื่อถือได้ของคอมพิวเตอร์ของคุณไม่ทำงานอย่างถูกต้อง"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ให้ลองทำดังต่อไปนี้:

1. เปิดแอป Office และ [ลงชื่อออก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) จากบัญชีผู้ใช้ใดๆที่มีอยู่   
2. การใช้**การตั้งค่า**Windows บัญชีผู้ใช้  >  **Accounts**  >  **อีเมลของ**บัญชีผู้ใช้ & เอาบัญชีที่ทำงานที่มีอยู่ออก 
3. การใช้**การตั้งค่า**Windows  >  **Accounts**  >  Access บัญชีที่**ทำงานหรือโรงเรียน**ให้ยกเลิกการเชื่อมต่อบัญชีผู้ใช้ที่มีอยู่ 
4. ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่ [เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)การ
5. ลอง [ใช้กระบวนการกู้คืนของผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของโมดูลของ PLATFORM (TPM) ที่เชื่อถือได้