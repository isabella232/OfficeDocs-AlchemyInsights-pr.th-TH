---
title: มีข้อผิดพลาดเกิดขึ้นในการตรวจสอบข้อผิดพลาดโทเค็นการเข้าถึงระหว่างการวิเคราะห์บนเดสก์ท็อป
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741292"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>เกิดข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ระหว่างการเตรียมใช้งาน Analytics บนเดสก์ท็อป

โดยปกติแล้วข้อผิดพลาดนี้จะสังเกตเห็นเมื่อโทเค็นการรับรองความถูกต้องหมดอายุ โดยปกติแล้วการรีเฟรชหน้าเว็บจะรีเฟรชโทเค็น อย่างไรก็ตามปัญหานี้สามารถยังคงมีอยู่ถ้ามีนโยบายการเข้าถึงแบบมีเงื่อนไขใดๆที่ใช้กับบัญชีที่ใช้ในการวิเคราะห์บนเดสก์ท็อปบนกระดาน คุณสามารถตรวจสอบแฟ้มบันทึกการเข้าสู่ระบบ AD Azure ในเว็บไซต์ Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้สำหรับบัญชีผู้ใช้สำหรับการเตรียมการของ Analytics บนเดสก์ท็อปหรือไม่

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงแบบมีเงื่อนไขให้เยี่ยมชม[แผนการปรับใช้การเข้าถึงแบบมีเงื่อนไขของคุณ](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)