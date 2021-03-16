---
title: แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO) ภายในองค์กร
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816347"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="caf4a-102">แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO) ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="caf4a-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="caf4a-103">เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียว (SSO) อย่างราบรื่น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="caf4a-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="caf4a-104">**ฉันจะเปิดคีย์การถอดรหัส Kerberos ของบัญชีคอมพิวเตอร์ AZUREADSSO ได้อย่างไร**</span><span class="sxs-lookup"><span data-stu-id="caf4a-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="caf4a-105">เราขอแนะนนะให้คุณใช้คีย์การถอดรหัส Kerberos อย่างน้อยทุก 30 วัน</span><span class="sxs-lookup"><span data-stu-id="caf4a-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="caf4a-106">To do this manually, [see how to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="caf4a-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="caf4a-107">**กําหนดค่า SSO อย่างราบรื่น**</span><span class="sxs-lookup"><span data-stu-id="caf4a-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="caf4a-108">เมื่อต้องการปรับใช้ SSO อย่างราบรื่น ให้ปฏิบัติตามขั้นตอนในการลงชื่อเข้าระบบครั้งเดียว [อย่างราบรื่นของ Azure Active Directory: การเริ่มต้นใช้งาน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)ด่วน</span><span class="sxs-lookup"><span data-stu-id="caf4a-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="caf4a-109">**ที่ปรึกษา**</span><span class="sxs-lookup"><span data-stu-id="caf4a-109">**Advisory**</span></span>

- <span data-ttu-id="caf4a-110">การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นของ[Azure Active Directory: Frequently asked](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) questions - ในบทความนี้ เราจะตอบถามที่ถามบ่อยเกี่ยวกับ Azure Active Directory Seamless Single Sign-On (Seamless SSO)</span><span class="sxs-lookup"><span data-stu-id="caf4a-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="caf4a-111">คอยตรวจสอบเนื้อหาใหม่อยู่</span><span class="sxs-lookup"><span data-stu-id="caf4a-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="caf4a-112">[ถามตอบ&ของ Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - บทความนี้มีข้อมูลเกี่ยวกับวิธีการสร้างการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="caf4a-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="caf4a-113">**แก้ไขปัญหา**</span><span class="sxs-lookup"><span data-stu-id="caf4a-113">**Troubleshoot**</span></span>

<span data-ttu-id="caf4a-114">[แก้ไขปัญหาการ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) ลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นของ Azure Active Directory - บทความนี้ช่วยให้คุณค้นหาข้อมูลการแก้ไขปัญหาทั่วไปเกี่ยวกับ Azure Active Directory (Azure AD Sign-On) การเข้าสู่ระบบครั้งเดียวอย่างราบรื่น (SSO อย่างราบรื่น)</span><span class="sxs-lookup"><span data-stu-id="caf4a-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







