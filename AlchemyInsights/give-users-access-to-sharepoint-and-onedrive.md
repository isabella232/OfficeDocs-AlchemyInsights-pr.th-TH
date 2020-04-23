---
title: ให้สิทธิ์ผู้ใช้เข้าถึง SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721848"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="35e06-102">ให้สิทธิ์ผู้ใช้เข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="35e06-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="35e06-103">ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="35e06-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="35e06-104">ตรวจสอบแดชบอร์ดสถานภาพบริการ</span><span class="sxs-lookup"><span data-stu-id="35e06-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="35e06-105">ถ้าคุณต้องการให้บุคคลในองค์กรของคุณสามารถลงชื่อเข้าใช้และใช้ SharePoint และ OneDrive ได้ คุณต้องเพิ่มบัญชีสําหรับบุคคลเหล่านั้น และตรวจสอบว่าบุคคลดังกล่าวมีสิทธิ์การใช้งานที่อนุญาตให้บุคคลเหล่านั้นเข้าถึง SharePoint และ OneDrive ได้</span><span class="sxs-lookup"><span data-stu-id="35e06-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="35e06-106">วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้อยู่ในศูนย์การจัดการ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="35e06-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="35e06-107">ไปที่หน้า[ผู้ใช้ที่ใช้งานอยู่ ใน ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/users)แล้วคลิก**เพิ่มผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="35e06-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="35e06-108">กรอกข้อมูลสําหรับผู้ใช้ และตรวจสอบให้แน่ใจว่าภายใต้**สิทธิ์การใช้งานผลิตภัณฑ์**สิทธิ์การใช้งานถูกมอบหมาย และ**SharePoint Online**ถูกเลือกไว้</span><span class="sxs-lookup"><span data-stu-id="35e06-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="35e06-109">โปรดทราบว่าถ้าคุณอนุญาตให้มีการแชร์ภายนอกในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="35e06-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="35e06-110">คุณไม่จําเป็นต้องให้สิทธิ์การใช้งานแก่ผู้ใช้ภายนอกเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="35e06-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="35e06-111">นอกจากนี้ คุณไม่จําเป็นต้องเพิ่มบัญชีสําหรับบัญชีเหล่านั้น เว้นแต่ว่าการใช้ร่วมกันถูกตั้งค่าเป็น "เฉพาะผู้ใช้ภายนอกที่มีอยู่เท่านั้น"</span><span class="sxs-lookup"><span data-stu-id="35e06-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="35e06-112">ในกรณีนี้ ถ้าบุคคลนั้นไม่ได้อยู่ในไดเรกทอรีขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="35e06-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

