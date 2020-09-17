---
title: มีข้อผิดพลาดในการตรวจสอบความถูกต้องของโทเค็นการเข้าถึงในระหว่างการใช้งาน Analytics บนเดสก์ท็อป
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783570"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>ข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ในระหว่างการปฐมนิเทศ Analytics บนเดสก์ท็อป

ข้อผิดพลาดนี้มักจะสังเกตเมื่อโทเค็นการรับรองความถูกต้องหมดอายุ โดยปกติแล้วการรีเฟรชหน้าจะรีเฟรชโทเค็น อย่างไรก็ตามปัญหานี้อาจยังคงมีอยู่ถ้ามีนโยบายการเข้าถึงตามเงื่อนไขที่นำไปใช้กับบัญชีผู้ใช้ในการวิเคราะห์บนเดสก์ท็อปบนกระดาน คุณสามารถตรวจสอบการลงชื่อเข้าใช้ Azure AD ในบันทึกในพอร์ทัล Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้สำหรับบัญชีผู้ใช้สำหรับปฐมนิเทศ Analytics บนเดสก์ท็อปหรือไม่

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงแบบมีเงื่อนไขให้เยี่ยมชม[วางแผนการปรับใช้การเข้าถึงตามเงื่อนไขของคุณ](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)