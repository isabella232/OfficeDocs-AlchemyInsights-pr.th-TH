---
title: รหัสกฎของโปรไฟล์การจัดสรร iOS 1029
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "322"
- "3100011"
ms.assetid: 14d30092-8cf5-4fe6-a2a3-8a337e96cb1c
ms.openlocfilehash: 07f98f96958e4897a3e14cef424cb0d7bd491dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43765936"
---
# <a name="ios-provisioning-profiles"></a><span data-ttu-id="58f2c-102">โปรไฟล์การจัดเตรียม iOS</span><span class="sxs-lookup"><span data-stu-id="58f2c-102">iOS Provisioning Profiles</span></span>

<span data-ttu-id="58f2c-103">สายของธุรกิจ Apple iOS ใช้แนวคิดของโปรไฟล์การจัดสรรซึ่งใช้ในการตรวจสอบความถูกต้องของแอปพลิเคชันและบังคับใช้นโยบายที่กําหนดไว้ในโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="58f2c-103">Apple iOS line-of-business uses the concept of a provisioning profile which is used to validate the integrity of the application and enforce policies defined in the profile.</span></span> <span data-ttu-id="58f2c-104">โปรไฟล์การจัดเตรียมเหล่านี้จะหมดอายุหลังจาก 12 เดือน ดังนั้นโปรไฟล์ใหม่ต้องเชื่อมโยงกับแอปที่ปรับใช้เพื่อให้แอปทํางานต่อไป</span><span class="sxs-lookup"><span data-stu-id="58f2c-104">These provisioning profiles expire after 12 months and so a new profile must be associated with the deployed app in order for the apps to continue to to run.</span></span>
  
<span data-ttu-id="58f2c-105">บทความต่อไปนี้จะอธิบายวิธีสร้างการเชื่อมโยงโปรไฟล์การจัดเตรียมใหม่กับแอป iOS LOB ที่ปรับใช้ผ่าน Intune:[ใช้โปรไฟล์การจัดเตรียมแอป iOS เพื่อป้องกันไม่ให้แอปของคุณหมดอายุ](https://docs.microsoft.com/intune/app-provisioning-profile-ios)</span><span class="sxs-lookup"><span data-stu-id="58f2c-105">The following article describes how to create associate a new provisioning profile with an iOS LOB app deployed through Intune: [Use iOS app provisioning profiles to prevent your apps from expiring](https://docs.microsoft.com/intune/app-provisioning-profile-ios)</span></span>
  