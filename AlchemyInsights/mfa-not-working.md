---
title: การตัดสินค้าจากคลังกับ MFA
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250184"
---
# <a name="issues-with-mfa"></a>การตัดสินค้าจากคลังกับ MFA
มีบางสิ่งที่จะตรวจสอบถ้าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย (MFA)

1. ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกใน Azure เว็บไซต์ไดเรกทอรีที่ใช้งานอยู่ ถ้าเป็นกรณีนี้ รับรองความถูกต้องพยายามให้ เฉพาะผู้ใช้จะสามารถโดยอัตโนมัติถูกปฏิเสธ [โปรดทำตามขั้นตอนในบทความนี้เพื่อยกเลิกบล็อกเหล่านั้น](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. ถ้าไม่ได้ช่วยบล็อกผู้ใช้ หรือผู้ใช้ที่ไม่ถูกบล็อคคุณสามารถลองตั้งค่าใหม่ MFA สำหรับผู้ใช้ และพวกเขาจะทำขั้นตอนการลงทะเบียนใหม่อีกครั้ง [โปรดทำตามขั้นตอนในบทความนี้](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณจะไม่สามารถล็อกอินไปยังไคลเอนต์ที่ไม่ใช่เบราว์เซอร์เช่น Outlook, Skype เป็นต้น บางที ADAL (Active Directory พิสูจน์ตัวจริงของไลบรารี) ไม่เปิดใช้งานบนการสมัครใช้งาน O365 ในกรณีนี้ คุณจะต้องเชื่อมต่อกับ Powershell แบบออนไลน์ของอัตราแลกเปลี่ยน และเรียกใช้ cmdlet นี้:  *ชุด-OrganizationConfig-OAuth2ClientProfileEnabled: $true*