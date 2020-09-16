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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="3b712-102">ปัญหาเกี่ยวกับ Azure MFA</span><span class="sxs-lookup"><span data-stu-id="3b712-102">Issues with Azure MFA</span></span>
<span data-ttu-id="3b712-103">มีสองสามสิ่งในการตรวจสอบว่าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องแบบหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="3b712-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="3b712-104">ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกในพอร์ทัลไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="3b712-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="3b712-105">ถ้าเป็นกรณีนี้ความพยายามในการรับรองความถูกต้องของผู้ใช้ที่เฉพาะเจาะจงจะถูกปฏิเสธโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="3b712-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="3b712-106">โปรดทำตามขั้นตอนในบทความนี้เพื่อยกเลิกการบล็อก</span><span class="sxs-lookup"><span data-stu-id="3b712-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="3b712-107">ถ้าการยกเลิกการบล็อกผู้ใช้ไม่ได้รับความช่วยเหลือหรือผู้ใช้ไม่ได้บล็อกคุณสามารถลองตั้งค่า MFA ใหม่สำหรับผู้ใช้และพวกเขาจะไปผ่านกระบวนการลงทะเบียนอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="3b712-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="3b712-108">โปรดทำตามขั้นตอนในบทความนี้</span><span class="sxs-lookup"><span data-stu-id="3b712-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="3b712-109">ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณไม่สามารถเข้าสู่ระบบไคลเอ็นต์ที่ไม่ใช่เบราว์เซอร์เช่น Outlook, Skype และอื่นๆอาจ ADAL (ไลบรารีการรับรองความถูกต้องของไดเรกทอรีที่ใช้งานอยู่) ไม่ได้เปิดใช้งานบนการสมัครใช้งาน O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="3b712-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="3b712-110">ในกรณีนี้คุณจะต้องเชื่อมต่อกับ Exchange Online Powershell และเรียกใช้ cmdlet นี้:  *ตั้งค่า-ชื่อ get-organizationconfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="3b712-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>