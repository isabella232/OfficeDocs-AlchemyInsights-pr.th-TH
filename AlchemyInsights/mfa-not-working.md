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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810503"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="0c168-102">ปัญหาเกี่ยวกับ Azure MFA</span><span class="sxs-lookup"><span data-stu-id="0c168-102">Issues with Azure MFA</span></span>
<span data-ttu-id="0c168-103">มีสองสิ่งที่ต้องตรวจสอบว่าผู้ใช้ไม่สามารถเข้าสู่ระบบโดยใช้การรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="0c168-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="0c168-104">ผู้ใช้ที่ได้รับผลกระทบอาจถูกบล็อกในพอร์ทัล Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0c168-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="0c168-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span><span class="sxs-lookup"><span data-stu-id="0c168-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="0c168-106">โปรดปฏิบัติตามขั้นตอนในบทความนี้เพื่อยกเลิกการบล็อก</span><span class="sxs-lookup"><span data-stu-id="0c168-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="0c168-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span><span class="sxs-lookup"><span data-stu-id="0c168-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="0c168-108">โปรดปฏิบัติตามขั้นตอนในบทความนี้</span><span class="sxs-lookup"><span data-stu-id="0c168-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="0c168-109">ถ้านี่เป็นครั้งแรกที่คุณเปิดใช้งาน MFA และผู้ใช้ของคุณไม่สามารถเข้าสู่ระบบไคลเอ็นต์ที่ไม่ใช่เบราว์เซอร์ เช่น Outlook, Skype และอื่นๆ อาจเปิดใช้งาน ADAL (Active Directory Authentication Library) ในการสมัครใช้งาน O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="0c168-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="0c168-110">ในกรณีนี้ คุณจะต้องเชื่อมต่อกับ Exchange Online Powershell และเรียกใช้ cmdlet นี้:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="0c168-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>