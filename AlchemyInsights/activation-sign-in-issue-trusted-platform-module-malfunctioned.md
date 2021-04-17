---
title: ปัญหาการเปิดใช้งาน/การลงชื่อเข้าใช้ - โมดูลแพลตฟอร์มที่เชื่อถือได้ผิดปกติ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822906"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>การแก้ไขข้อความ "โมดูลแพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณมีฟังก์ชันการฟังก์ชันไม่ถูกต้อง" ของแอป Microsoft 365

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองวิธีต่อไปนี้:

1. เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่   
2. การใช้บัญชี **บัญชี**  >  **การตั้งค่า**  >  **Windows &อีเมล** ลบบัญชีที่งานที่มีอยู่ออก 
3. การใช้ บัญชี **การตั้งค่า** Windows  >    >  **เข้าถึงบัญชีที่โรงเรียน** หรือที่โรงเรียน ยกเลิกการเชื่อมต่อบัญชีที่มีอยู่ 
4. รีเซ็ตสถานะการเปิดใช้งาน Office [เรียนรู้วิธีการ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)
5. ลองกระบวนการ [กู้คืนผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของ Trusted Platform Module (TPM)