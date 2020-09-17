---
title: วิธีเปิดใช้งาน SSO อย่างราบรื่น
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780546"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="5d157-102">วิธีเปิดใช้งาน SSO อย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="5d157-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="5d157-103">เปิดใช้งาน SSO อย่างราบรื่นผ่าน[AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="5d157-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="5d157-104">ถ้าคุณกำลังทำการติดตั้งใหม่ของ Azure AD Connect ให้เลือก[เส้นทางการติดตั้งแบบกำหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)</span><span class="sxs-lookup"><span data-stu-id="5d157-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="5d157-105">ที่หน้า**ลงชื่อเข้าใช้ของผู้ใช้**ให้เลือกตัวเลือก**เปิดใช้งานการลงชื่อเข้าใช้ครั้งเดียว**</span><span class="sxs-lookup"><span data-stu-id="5d157-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="5d157-106">เมื่อต้องการตรวจสอบว่าคุณได้เปิดใช้งานอย่างราบรื่น SSO อย่างถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="5d157-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="5d157-107">ลงชื่อเข้าใช้ [ศูนย์การจัดการไดเรกทอรีของ Azure ที่ใช้งานอยู่](https://aad.portal.azure.com) ในฐานะผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="5d157-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="5d157-108">เลือก **Azure Active directory** ในบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="5d157-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="5d157-109">ตรวจสอบว่า **เปิดใช้งาน**การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="5d157-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="5d157-110">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[ไดเรกทอรีที่ใช้งานอยู่ของ Azure การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น: เริ่มต้น](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)</span><span class="sxs-lookup"><span data-stu-id="5d157-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  