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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="0b7f8-102">ปัญหาเกี่ยวกับ MFA</span><span class="sxs-lookup"><span data-stu-id="0b7f8-102">Issues with Azure MFA</span></span>
<span data-ttu-id="0b7f8-103">มีสองสิ่งที่ต้องตรวจสอบว่าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="0b7f8-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="0b7f8-104">ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกในเว็บไซต์ไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="0b7f8-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="0b7f8-105">หากเป็นกรณีนี้ความพยายามในการตรวจสอบสิทธิ์สำหรับผู้ใช้ที่เฉพาะเจาะจงนั้นจะถูกปฏิเสธโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="0b7f8-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="0b7f8-106">โปรดทำตามขั้นตอนในบทความนี้เพื่อยกเลิกการบล็อก</span><span class="sxs-lookup"><span data-stu-id="0b7f8-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="0b7f8-107">ถ้าการบล็อกผู้ใช้ไม่ได้ช่วยเหลือหรือผู้ใช้ไม่ได้ถูกบล็อกคุณสามารถลองรีเซ็ต MFA สำหรับผู้ใช้และพวกเขาจะไปผ่านขั้นตอนการลงทะเบียนอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="0b7f8-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="0b7f8-108">โปรดทำตามขั้นตอนในบทความนี้</span><span class="sxs-lookup"><span data-stu-id="0b7f8-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="0b7f8-109">ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณจะไม่สามารถเข้าสู่ระบบไคลเอนต์ที่ไม่ใช่เบราว์เซอร์เช่น Outlook, Skype, ฯลฯอาจจะ ADAL (ไลบรารีการรับรองความถูกต้องไดเรกทอรีที่ใช้งานอยู่) ไม่ได้เปิดใช้งานในการสมัครสมาชิก O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="0b7f8-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="0b7f8-110">ในกรณีนี้คุณจะต้องเชื่อมต่อกับ Powershell แบบออนไลน์ของอัตราแลกเปลี่ยนและเรียกใช้ cmdlet นี้:  *ตั้งค่าองค์กร OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="0b7f8-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>