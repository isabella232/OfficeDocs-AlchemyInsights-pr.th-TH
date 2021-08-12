---
title: มีข้อผิดพลาดการตรวจสอบความถูกต้องของข้อผิดพลาดโทเค็นการเข้าถึงระหว่างการวิเคราะห์เดสก์ท็อปบนบอร์ด
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
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946634"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>ข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ระหว่างการออนบอร์ดการวิเคราะห์เดสก์ท็อป

โดยปกติแล้วจะพบข้อผิดพลาดนี้เมื่อโทเค็นการรับรองความถูกต้องหมดอายุ โดยปกติแล้ว รีเฟรชหน้าจะรีเฟรชโทเค็น อย่างไรก็ตาม ปัญหานี้สามารถคงอยู่ได้ถ้ามีนโยบายการเข้าถึงตามเงื่อนไขที่ปรับใช้กับบัญชีที่ใช้กับการวิเคราะห์เดสก์ท็อปบนบอร์ด คุณสามารถตรวจทานแฟ้มบันทึกการลงชื่อเข้าใช้ Azure AD ในพอร์ทัล Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้บัญชีที่ใช้กับการออนบอร์ดบนเดสก์ท็อปหรือไม่

For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).