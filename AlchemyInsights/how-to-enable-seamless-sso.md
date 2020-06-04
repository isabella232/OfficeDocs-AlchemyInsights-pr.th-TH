---
title: วิธีการเปิดใช้งาน SSO แบบไร้รอยต่อ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 3cf751bc42322067c4b7cd9b5facb933430f2b87
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "36663898"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="f70b6-102">วิธีการเปิดใช้งาน SSO แบบไร้รอยต่อ</span><span class="sxs-lookup"><span data-stu-id="f70b6-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="f70b6-103">เปิดใช้งาน SSO ที่ราบรื่นผ่าน[การเชื่อมต่อโฆษณา Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="f70b6-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="f70b6-104">ถ้าคุณกําลังทําการติดตั้งใหม่ของ Azure AD Connect ให้เลือก[เส้นทางการติดตั้งแบบกําหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)</span><span class="sxs-lookup"><span data-stu-id="f70b6-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="f70b6-105">ที่หน้า**ลงชื่อเข้าใช้ของผู้ใช้**ให้เลือกตัวเลือก**เปิดใช้งานการลงชื่อเข้าใช้ครั้งเดียว**</span><span class="sxs-lookup"><span data-stu-id="f70b6-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="f70b6-106">เมื่อต้องการตรวจสอบว่า คุณได้เปิดใช้งาน SSO แบบไม่มีรอยต่ออย่างถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="f70b6-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="f70b6-107">เข้าสู่ระบบไปยัง[ศูนย์การจัดการ Azure Active Directory](https://aad.portal.azure.com)เป็นผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="f70b6-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="f70b6-108">เลือก**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**ในบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="f70b6-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="f70b6-109">ตรวจสอบว่าการลงชื่อเข้าระบบครั้งเดียวแบบไม่มีรอยต่อ**ถูกเปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="f70b6-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="f70b6-110">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดูที่[Azure Active Directory แบบครั้งเดียวที่ราบรื่น: เริ่มต้นใช้งานด่วน](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)</span><span class="sxs-lookup"><span data-stu-id="f70b6-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  