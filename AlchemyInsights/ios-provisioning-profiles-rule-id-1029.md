---
title: รหัสของกฎโพรไฟล์ Provisioning 1029 iOS
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 14d30092-8cf5-4fe6-a2a3-8a337e96cb1c
ms.openlocfilehash: 54f84daa0023296c6a979e7559eb5bbdd8eb7054
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493156"
---
# <a name="ios-provisioning-profiles"></a><span data-ttu-id="defbf-102">โพรไฟล์การเตรียมใช้งาน iOS</span><span class="sxs-lookup"><span data-stu-id="defbf-102">iOS Provisioning Profiles</span></span>

<span data-ttu-id="defbf-p101">เครื่องคอมพิวเตอร์ Apple iOS บรรทัดทางธุรกิจใช้แนวคิดของการเตรียมใช้งานโพรไฟล์ซึ่งใช้ในการตรวจสอบความสมบูรณ์ของแอพลิเคชัน และบังคับใช้นโยบายที่กำหนดไว้ในโพรไฟล์ สิ่งเหล่านี้การเตรียมใช้งานโพรไฟล์หมดอายุหลังจาก 12 เดือน และดังนั้น ต้องเกี่ยวข้องกับโปรแกรมประยุกต์ที่ใช้งานจริงในใบสั่งสำหรับโปรแกรมประยุกต์เพื่อดำเนินต่อเพื่อเรียกใช้ส่วนกำหนดค่าใหม่</span><span class="sxs-lookup"><span data-stu-id="defbf-p101">Apple iOS line-of-business uses the concept of a provisioning profile which is used to validate the integrity of the application and enforce policies defined in the profile. These provisioning profiles expire after 12 months and so a new profile must be associated with the deployed app in order for the apps to continue to to run.</span></span>
  
<span data-ttu-id="defbf-105">บทความต่อไปนี้อธิบายวิธีการสร้างการเชื่อมโยงการเตรียมใช้งานใหม่ของโพรไฟล์ ด้วยการ iOS app LOB ที่ปรับใช้ผ่านทาง Intune:[ใช้ iOS app เตรียมใช้งานโพรไฟล์เพื่อป้องกันไม่ให้โปรแกรมประยุกต์ของคุณจากการหมดอายุ](https://docs.microsoft.com/intune/app-provisioning-profile-ios)</span><span class="sxs-lookup"><span data-stu-id="defbf-105">The following article describes how to create associate a new provisioning profile with an iOS LOB app deployed through Intune: [Use iOS app provisioning profiles to prevent your apps from expiring](https://docs.microsoft.com/intune/app-provisioning-profile-ios)</span></span>
  

