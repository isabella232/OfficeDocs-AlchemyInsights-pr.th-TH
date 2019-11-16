---
title: ปัญหาเกี่ยวกับ MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768856"
---
# <a name="issues-with-azure-mfa"></a>ปัญหาเกี่ยวกับ MFA
มีสองสิ่งที่ต้องตรวจสอบว่าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย (MFA)

1. ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกในเว็บไซต์ไดเรกทอรีที่ใช้งานอยู่ของ Azure หากเป็นกรณีนี้ความพยายามในการตรวจสอบสิทธิ์สำหรับผู้ใช้ที่เฉพาะเจาะจงนั้นจะถูกปฏิเสธโดยอัตโนมัติ [โปรดทำตามขั้นตอนในบทความนี้เพื่อยกเลิกการบล็อก](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. ถ้าการบล็อกผู้ใช้ไม่ได้ช่วยเหลือหรือผู้ใช้ไม่ได้ถูกบล็อกคุณสามารถลองรีเซ็ต MFA สำหรับผู้ใช้และพวกเขาจะไปผ่านขั้นตอนการลงทะเบียนอีกครั้ง [โปรดทำตามขั้นตอนในบทความนี้](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณจะไม่สามารถเข้าสู่ระบบไคลเอนต์ที่ไม่ใช่เบราว์เซอร์เช่น Outlook, Skype, ฯลฯอาจจะ ADAL (ไลบรารีการรับรองความถูกต้องไดเรกทอรีที่ใช้งานอยู่) ไม่ได้เปิดใช้งานในการสมัครสมาชิก O365 ของคุณ ในกรณีนี้คุณจะต้องเชื่อมต่อกับ Powershell แบบออนไลน์ของอัตราแลกเปลี่ยนและเรียกใช้ cmdlet นี้:  *ตั้งค่าองค์กร OAuth2ClientProfileEnabled: $true*