---
title: วิธีการเปิดใช้งาน SSO อย่างราบรื่น
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825750"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="21b5c-102">วิธีการเปิดใช้งาน SSO อย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="21b5c-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="21b5c-103">เปิดใช้งาน SSO อย่างราบรื่น[ผ่าน Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="21b5c-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="21b5c-104">ถ้าคุณติดตั้ง Azure AD Connect ใหม่ ให้เลือกเส้นทางการติดตั้ง [แบบปรับแต่ง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)เอง</span><span class="sxs-lookup"><span data-stu-id="21b5c-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="21b5c-105">ที่ **หน้าลงชื่อเข้าใช้ของผู้ใช้** ให้เลือกตัวเลือก **เปิดใช้งานการเข้าสู่ระบบโดย** ลงชื่อเข้าใช้ครั้งเดียว</span><span class="sxs-lookup"><span data-stu-id="21b5c-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="21b5c-106">เมื่อต้องการตรวจสอบว่าคุณได้เปิดใช้งาน SSO อย่างราบรื่นอย่างถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="21b5c-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="21b5c-107">ลงชื่อเข้าใช้ศูนย์การจัดการ [Azure Active Directory](https://aad.portal.azure.com) ในฐานะผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="21b5c-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="21b5c-108">เลือก **Azure Active Directory** ในบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="21b5c-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="21b5c-109">ตรวจสอบว่า เปิดใช้งานการเข้าสู่ระบบโดย **ลงชื่อเข้าใช้ครั้งเดียวอย่าง** ราบรื่น</span><span class="sxs-lookup"><span data-stu-id="21b5c-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="21b5c-110">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [การลงชื่อเข้าระบบครั้งเดียวอย่าง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)ราบรื่นของ Azure Active Directory: เริ่มต้นใช้งานด่วน</span><span class="sxs-lookup"><span data-stu-id="21b5c-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  