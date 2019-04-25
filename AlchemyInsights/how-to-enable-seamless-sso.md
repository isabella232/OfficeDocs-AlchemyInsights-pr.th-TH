---
title: วิธีการเปิดใช้งาน SSO อย่างราบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 5a6d34c5dc5cca307cd085011a88cf7171d207ad
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408666"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="4ccd7-102">วิธีการเปิดใช้งาน SSO อย่างราบ</span><span class="sxs-lookup"><span data-stu-id="4ccd7-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="4ccd7-103">เปิดใช้งาน SSO อย่างราบผ่าน[การเชื่อมต่อ Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="4ccd7-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="4ccd7-104">ถ้าคุณกำลังทำการติดตั้งใหม่ของการเชื่อมต่อ AD Azure เลือก[เส้นทางการติดตั้งแบบกำหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)</span><span class="sxs-lookup"><span data-stu-id="4ccd7-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="4ccd7-105">หน้า**ผู้ใช้ในการเข้าระบบ**เลือกตัวเลือกการ**เปิดใช้งานสู่ระบบแบบครั้งเดียว**</span><span class="sxs-lookup"><span data-stu-id="4ccd7-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span> 
  
<span data-ttu-id="4ccd7-106">เมื่อต้องการตรวจสอบว่า คุณได้เปิดใช้งานอย่างราบ SSO อย่างถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="4ccd7-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="4ccd7-107">เข้าสู่ระบบของ[ไดเรกทอรีที่ใช้งานอยู่ของ Azure กับศูนย์ดูแล](https://aad.portal.azure.com)ฐานะเป็นผู้ดูแลส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="4ccd7-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span> 
    
2. <span data-ttu-id="4ccd7-108">เลือก**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**ในบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="4ccd7-108">Select **Azure Active Directory** in the left pane.</span></span> 
    
3. <span data-ttu-id="4ccd7-109">ตรวจสอบว่า สขึ้นหนึ่งเข้าสู่ระบบถูก**เปิดใช้งาน**หรือไม่</span><span class="sxs-lookup"><span data-stu-id="4ccd7-109">Verify that Seamless single sign-on is **Enabled**.</span></span>
    
<span data-ttu-id="4ccd7-110">เมื่อต้องการเรียนรู้เพิ่มเติม ดู[Azure Active Directory อย่างราบเดียวเข้าสู่ระบบ: เริ่มต้นอย่างรวดเร็ว](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)</span><span class="sxs-lookup"><span data-stu-id="4ccd7-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  

