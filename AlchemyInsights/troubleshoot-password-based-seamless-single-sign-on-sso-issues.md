---
title: แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น (SSO) โดยใช้รหัสผ่าน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714889"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="75b30-102">แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น (SSO) โดยใช้รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="75b30-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="75b30-103">เมื่อต้องการเรียนรู้พื้นฐานของ SSO ที่ใช้รหัสผ่าน ให้ดูการรับรองความถูก[ต้องโดยใช้รหัสผ่านด้วย Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="75b30-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="75b30-104">**กําหนดค่า SSO ที่ใช้รหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="75b30-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="75b30-105">[กําหนดค่าการลงชื่อเข้าระบบครั้งเดียว](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) โดยใช้รหัสผ่าน - บทความนี้มีรายละเอียดเพิ่มเติมเกี่ยวกับตัวเลือก SSO ที่ใช้รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="75b30-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="75b30-106">ถ้าแอปพลิเคชันที่คุณเพิ่มต้องการการกําหนดค่าแบบกําหนดเองและคุณต้องใช้ SSO ที่ใช้รหัสผ่าน บทความนี้มีไว้เพื่อคุณ</span><span class="sxs-lookup"><span data-stu-id="75b30-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="75b30-107">[กําหนดค่าการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านของแอปภายในเครื่อง](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - พร็อกซีแอปพลิเคชันสนับสนุนโหมดการลงชื่อเข้าระบบครั้งเดียวหลายโหมด</span><span class="sxs-lookup"><span data-stu-id="75b30-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="75b30-108">การลงชื่อเข้าใช้ด้วยรหัสผ่านมีไว้เพื่อแอปพลิเคชันที่ใช้การรวมกันของชื่อผู้ใช้/รหัสผ่านเพื่อการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="75b30-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="75b30-109">เมื่อคุณกําหนดค่าการลงชื่อเข้าใช้ด้วยรหัสผ่านของแอปพลิเคชันของคุณ ผู้ใช้ของคุณจะต้องลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กรหนึ่งครั้ง</span><span class="sxs-lookup"><span data-stu-id="75b30-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="75b30-110">หลังจากนั้น Azure Active Directory จะจัดเก็บข้อมูลการลงชื่อเข้าใช้และมอบข้อมูลนั้นไปยังแอปพลิเคชันโดยอัตโนมัติเมื่อผู้ใช้ของคุณเข้าถึงจากระยะไกล</span><span class="sxs-lookup"><span data-stu-id="75b30-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="75b30-111">คุณควรเผยแพร่และทดสอบแอปของคุณด้วยพร็อกซีแอปพลิเคชันแล้ว</span><span class="sxs-lookup"><span data-stu-id="75b30-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="75b30-112">ถ้าไม่ ให้ปฏิบัติตามขั้นตอนใน [ประกาศแอปพลิเคชันโดยใช้พร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) แอปพลิเคชัน Azure AD จากนั้นให้กําหนดค่า SSO ที่ยึดตามรหัสผ่านของคุณต่อไป</span><span class="sxs-lookup"><span data-stu-id="75b30-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="75b30-113">เมื่อต้องการแก้ไขปัญหา SSO ที่ยึดตามรหัสผ่าน ให้ดู [แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านใน Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="75b30-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
