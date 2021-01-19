---
title: ปัญหาในการลงชื่อออก
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901299"
---
# <a name="sign-out-issues"></a><span data-ttu-id="2eb5c-102">ปัญหาในการลงชื่อออก</span><span class="sxs-lookup"><span data-stu-id="2eb5c-102">Sign-out issues</span></span>

<span data-ttu-id="2eb5c-103">เมื่อต้องการแก้ไขปัญหาที่เกี่ยวข้องกับการออกจากระบบให้ดำเนินการตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="2eb5c-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="2eb5c-104">ถ้าคุณหรือผู้ใช้ได้รับการบันทึกหรือออกจากแอปพลิเคชันให้ทำตามคำแนะนำในบทความที่[กำหนดค่าการจัดการเซสชันการรับรองความถูกต้องด้วยการเข้าถึงตามเงื่อนไขหรือมีการกำหนดระยะเวลาที่กำหนด](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime)ไว้[ใน Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="2eb5c-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="2eb5c-105">ข้อผิดพลาดการลงชื่อเข้าใช้อื่นๆส่วนใหญ่หรือปัญหาสามารถแก้ไขได้โดยการแก้ไขปัญหาการรวม Azure Active Directory (Azure AD) ที่มีแอปพลิเคชันที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="2eb5c-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="2eb5c-106">คุณสามารถค้นหาคำแนะนำสำหรับการรวมที่เฉพาะเจาะจงได้โดยไปที่ [คอลเลกชันของบทช่วยสอนสำหรับการรวมแอปพลิเคชันด้วย Azure Active directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)รวมถึง:</span><span class="sxs-lookup"><span data-stu-id="2eb5c-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="2eb5c-107">บทช่วยสอนเกี่ยวกับแอปพลิเคชัน SaaS</span><span class="sxs-lookup"><span data-stu-id="2eb5c-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="2eb5c-108">บทช่วยสอนการลงชื่อเข้าระบบครั้งเดียว</span><span class="sxs-lookup"><span data-stu-id="2eb5c-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="2eb5c-109">บทช่วยสอนการเตรียมใช้งานของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="2eb5c-109">User-provisioning tutorials</span></span>