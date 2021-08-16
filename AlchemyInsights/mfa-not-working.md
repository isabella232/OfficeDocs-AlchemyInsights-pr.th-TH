---
title: ปัญหาเกี่ยวกับ MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098621"
---
# <a name="issues-with-azure-mfa"></a>ปัญหาเกี่ยวกับ Azure MFA
มีสองสิ่งที่ต้องตรวจสอบว่าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)

1. ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกในAzure Active Directoryของคุณ If that is the case, Authentication attempts for that specific user will be automatically denied. [โปรดปฏิบัติตามขั้นตอนในบทความนี้เพื่อยกเลิกการบล็อก](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again. [โปรดปฏิบัติตามขั้นตอนในบทความนี้](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณไม่สามารถเข้าสู่ระบบไคลเอ็นต์ที่ไม่ใช่เบราว์เซอร์ เช่น Outlook, Skype และอื่นๆ อาจเปิดใช้งาน ADAL (ไลบรารีการรับรองความถูกต้อง Active Directory) บนการสมัครใช้งาน O365 ของคุณ ในกรณีนี้ คุณจะต้องเชื่อมต่อกับ Powershell Exchange Online cmdlet นี้: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*