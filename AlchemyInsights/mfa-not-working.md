---
title: ปัญหาเกี่ยวกับ MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755150"
---
# <a name="issues-with-azure-mfa"></a>ปัญหาเกี่ยวกับ Azure MFA
มีสองสามสิ่งในการตรวจสอบว่าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องแบบหลายปัจจัย (MFA)

1. ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกในพอร์ทัลไดเรกทอรีที่ใช้งานอยู่ของ Azure ถ้าเป็นกรณีนี้ความพยายามในการรับรองความถูกต้องของผู้ใช้ที่เฉพาะเจาะจงจะถูกปฏิเสธโดยอัตโนมัติ [โปรดทำตามขั้นตอนในบทความนี้เพื่อยกเลิกการบล็อก](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. ถ้าการยกเลิกการบล็อกผู้ใช้ไม่ได้รับความช่วยเหลือหรือผู้ใช้ไม่ได้บล็อกคุณสามารถลองตั้งค่า MFA ใหม่สำหรับผู้ใช้และพวกเขาจะไปผ่านกระบวนการลงทะเบียนอีกครั้ง [โปรดทำตามขั้นตอนในบทความนี้](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณไม่สามารถเข้าสู่ระบบไคลเอ็นต์ที่ไม่ใช่เบราว์เซอร์เช่น Outlook, Skype และอื่นๆอาจ ADAL (ไลบรารีการรับรองความถูกต้องของไดเรกทอรีที่ใช้งานอยู่) ไม่ได้เปิดใช้งานบนการสมัครใช้งาน O365 ของคุณ ในกรณีนี้คุณจะต้องเชื่อมต่อกับ Exchange Online Powershell และเรียกใช้ cmdlet นี้:  *ตั้งค่า-ชื่อ get-organizationconfig-OAuth2ClientProfileEnabled: $true*