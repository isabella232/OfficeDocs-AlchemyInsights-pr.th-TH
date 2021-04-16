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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813707"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>ข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ระหว่างการออนบอร์ดการวิเคราะห์เดสก์ท็อป

โดยปกติแล้วจะพบข้อผิดพลาดนี้เมื่อโทเค็นการรับรองความถูกต้องหมดอายุ โดยปกติแล้ว รีเฟรชหน้าจะรีเฟรชโทเค็น อย่างไรก็ตาม ปัญหานี้สามารถคงอยู่ได้ถ้ามีนโยบายการเข้าถึงตามเงื่อนไขที่ปรับใช้กับบัญชีที่ใช้กับการวิเคราะห์เดสก์ท็อปบนบอร์ด คุณสามารถตรวจทานแฟ้มบันทึกการลงชื่อเข้าใช้ Azure AD ในพอร์ทัล Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้บัญชีที่ใช้กับการออนบอร์ดบนเดสก์ท็อปหรือไม่

For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).