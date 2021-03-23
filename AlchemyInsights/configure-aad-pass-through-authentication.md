---
title: กําหนดค่าการรับรองความถูกต้องแบบพาส-ทะลุผ่านของ Azure Active Directory
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037533"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="0c03e-102">กําหนดค่าการรับรองความถูกต้องแบบพาส-ทะลุผ่านของ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0c03e-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="0c03e-103">ต่อไปนี้เป็นแนวทางบางส่วนเพื่อช่วยให้คุณกําหนดค่าการรับรองความถูกต้องแบบพาส-ผ่าน:</span><span class="sxs-lookup"><span data-stu-id="0c03e-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="0c03e-104">**เมื่อต้องการตั้งค่า Azure Active Directory Connect**: การซิงค์ผู้ใช้กับ [คู่มือ](https://admin.microsoft.com/AdminPortal/Home) ไดเรกทอรีของคุณจะช่วยให้คุณกําหนดค่าการซิงโครไนซ์แฮชของรหัสผ่านหรือการรับรองความถูกต้องแบบพาส-ผ่าน</span><span class="sxs-lookup"><span data-stu-id="0c03e-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="0c03e-105">การกําหนดค่านี้จะให้ผู้ใช้ลงชื่อเข้าใช้อีเมลของพวกเขาและ Active Directory (ตัวควบคุมโดเมน) ภายในองค์กรของคุณโดยใช้รหัสผ่านเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="0c03e-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="0c03e-106">การซิงค์ [ผู้ใช้กับคู่มือไดเรกทอรีของคุณ](https://admin.microsoft.com/AdminPortal/Home) ยังครอบคลุมถึงการลงชื่อเข้าใช้การติดต่อกับภายนอกด้วย Active Directory Federation Services (AD FS) ด้วย</span><span class="sxs-lookup"><span data-stu-id="0c03e-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="0c03e-107">เมื่อต้องการตั้งค่าฟีเจอร์ **Azure:** คู่มือการตั้งค่า [Azure AD](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup)จะแนะนเกี่ยวกับการตั้งค่าฟีเจอร์ใน Azure Active Directory Basic เช่น การจัดการการเข้าถึงแบบกลุ่ม การตั้งค่ารหัสผ่านใหม่แบบบริการตนเองของแอประบบคลาวด์ และพร็อกซีแอปพลิเคชัน Azure Active Directory เพื่อเผยแพร่เว็บแอปภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="0c03e-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


