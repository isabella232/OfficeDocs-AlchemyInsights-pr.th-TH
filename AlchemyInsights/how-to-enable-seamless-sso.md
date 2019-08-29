---
title: วิธีการเปิดใช้งาน SSO ไม่มีรอยต่อ
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36663898"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="68160-102">วิธีการเปิดใช้งาน SSO ไม่มีรอยต่อ</span><span class="sxs-lookup"><span data-stu-id="68160-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="68160-103">เปิดใช้งาน SSO ที่ไม่มีรอยต่อผ่านการ[เชื่อมต่อ AD Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="68160-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="68160-104">ถ้าคุณกำลังทำการติดตั้งใหม่ของการเชื่อมต่อ AD Azure เลือก[เส้นทางการติดตั้งแบบกำหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)</span><span class="sxs-lookup"><span data-stu-id="68160-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="68160-105">ที่หน้า**เข้าสู่ระบบของผู้ใช้**ให้เลือกตัวเลือกการ**เปิดใช้งานการเข้าสู่ระบบแบบครั้งเดียว**</span><span class="sxs-lookup"><span data-stu-id="68160-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="68160-106">เพื่อตรวจสอบว่าคุณได้เปิดใช้งาน SSO อย่างราบรื่นแล้ว:</span><span class="sxs-lookup"><span data-stu-id="68160-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="68160-107">เข้าสู่ระบบไปยัง[ศูนย์การจัดการไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://aad.portal.azure.com)เป็นผู้ดูแลส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="68160-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="68160-108">เลือก**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**ในบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="68160-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="68160-109">ตรวจสอบว่า**เปิดใช้งาน**การเข้าสู่ระบบแบบครั้งเดียวอย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="68160-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="68160-110">เมื่อต้องการเรียนรู้เพิ่มเติมโปรดดูที่[Azure ที่ใช้งานอยู่การเข้าสู่ระบบแบบครั้งเดียว: เริ่มต้นอย่างรวดเร็ว](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)</span><span class="sxs-lookup"><span data-stu-id="68160-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  