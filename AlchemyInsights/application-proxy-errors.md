---
title: การแก้ไขปัญหาข้อผิดพลาดที่เกี่ยวข้องกับพร็อกซีแอปพลิเคชัน
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
- "9004356"
- "9686"
ms.openlocfilehash: fe0bae35942af9925e8a5f90f966e204d7f84fd2
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038171"
---
# <a name="troubleshoot-errors-related-to-application-proxy"></a><span data-ttu-id="74bfb-102">การแก้ไขปัญหาข้อผิดพลาดที่เกี่ยวข้องกับพร็อกซีแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="74bfb-102">Troubleshoot errors related to Application Proxy</span></span>

- <span data-ttu-id="74bfb-103">เมื่อต้องการเรียนรู้เกี่ยวกับข้อผิดพลาดทั่วไปที่ได้จากการตั้งค่าและการกําหนดค่า Kerberos และข้อเสนอแนะเกี่ยวกับการแก้ปัญหา ให้ดู การแก้ไขปัญหาพร็อกซีแอปพลิเคชัน [และข้อความ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-troubleshoot#kerberos-errors)แสดงข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="74bfb-103">To learn about the more common errors that come from Kerberos setup and configuration, and suggestions for resolution, see [Troubleshoot Application Proxy problems and error messages](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-troubleshoot#kerberos-errors).</span></span>
- <span data-ttu-id="74bfb-104">For App Proxy 404 errors, see [App page doesn't display correctly for Application Proxy app | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-page-appearance-broken-problem)</span><span class="sxs-lookup"><span data-stu-id="74bfb-104">For App Proxy 404 errors, see [App page doesn't display correctly for Application Proxy app | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-page-appearance-broken-problem).</span></span>
- <span data-ttu-id="74bfb-105">ใน Azure Active Directory (Azure AD) การกําหนดค่าแอปพลิเคชันภายในองค์กรจํานวนมากอาจไม่สามารถจัดการได้รวดเร็วและมีความเสี่ยงที่ไม่จําเป็นต่อข้อผิดพลาดในการกําหนดค่า ถ้าจํานวนมากต้องการการตั้งค่าเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="74bfb-105">In Azure Active Directory (Azure AD), configuring a large number of on-premises applications can quickly become unmanageable and introduces unnecessary risks for configuration errors if many of them require the same settings.</span></span> <span data-ttu-id="74bfb-106">ด้วย [พร็อกซีแอปพลิเคชัน Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy)คุณสามารถแก้ไขปัญหานี้โดยใช้การประกาศแอปพลิเคชันอักขระตัวแทนเพื่อเผยแพร่และจัดการแอปพลิเคชันมากมายในครั้งเดียว</span><span class="sxs-lookup"><span data-stu-id="74bfb-106">With [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy), you can address this issue by using wildcard application publishing to publish and manage many applications at once.</span></span> <span data-ttu-id="74bfb-107">For more information, see [Wildcard applications in the Azure AD Application Proxy | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)</span><span class="sxs-lookup"><span data-stu-id="74bfb-107">For more information, see [Wildcard applications in the Azure AD Application Proxy | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard).</span></span>
