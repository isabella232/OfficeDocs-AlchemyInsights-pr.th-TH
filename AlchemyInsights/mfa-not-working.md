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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545203"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="4d7d1-102">การตัดสินค้าจากคลังกับ MFA</span><span class="sxs-lookup"><span data-stu-id="4d7d1-102">Issues with MFA</span></span>
<span data-ttu-id="4d7d1-103">มีบางสิ่งที่จะตรวจสอบถ้าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="4d7d1-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="4d7d1-104">ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกใน Azure เว็บไซต์ไดเรกทอรีที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="4d7d1-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="4d7d1-105">ถ้าเป็นกรณีนี้ รับรองความถูกต้องพยายามให้ เฉพาะผู้ใช้จะสามารถโดยอัตโนมัติถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="4d7d1-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="4d7d1-106">โปรดทำตามขั้นตอนในบทความนี้เพื่อยกเลิกบล็อกเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="4d7d1-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="4d7d1-107">ถ้าไม่ได้ช่วยบล็อกผู้ใช้ หรือผู้ใช้ที่ไม่ถูกบล็อคคุณสามารถลองตั้งค่าใหม่ MFA สำหรับผู้ใช้ และพวกเขาจะทำขั้นตอนการลงทะเบียนใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="4d7d1-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="4d7d1-108">โปรดทำตามขั้นตอนในบทความนี้</span><span class="sxs-lookup"><span data-stu-id="4d7d1-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="4d7d1-109">ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณจะไม่สามารถล็อกอินไปยังไคลเอนต์ที่ไม่ใช่เบราว์เซอร์เช่น Outlook, Skype เป็นต้น บางที ADAL (Active Directory พิสูจน์ตัวจริงของไลบรารี) ไม่เปิดใช้งานบนการสมัครใช้งาน O365</span><span class="sxs-lookup"><span data-stu-id="4d7d1-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="4d7d1-110">ในกรณีนี้ คุณจะต้องเชื่อมต่อกับ Powershell แบบออนไลน์ของอัตราแลกเปลี่ยน และเรียกใช้ cmdlet นี้:  *ชุด-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="4d7d1-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>