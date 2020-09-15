---
title: ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive แก่ผู้ใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677226"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="c36a8-102">ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive แก่ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="c36a8-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="c36a8-103">ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="c36a8-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="c36a8-104">ตรวจสอบแดชบอร์ดสถานภาพบริการ</span><span class="sxs-lookup"><span data-stu-id="c36a8-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="c36a8-105">ถ้าคุณต้องการให้บุคคลในองค์กรของคุณสามารถลงชื่อเข้าใช้และใช้ SharePoint และ OneDrive คุณจำเป็นต้องเพิ่มบัญชีผู้ใช้เหล่านั้นและตรวจสอบให้แน่ใจว่ามีสิทธิ์การใช้งานที่ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="c36a8-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="c36a8-106">วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้อยู่ในศูนย์การจัดการ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="c36a8-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="c36a8-107">ไปที่[หน้าผู้ใช้ที่ใช้งานอยู่ในศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/users)แล้วคลิก**เพิ่มผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="c36a8-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="c36a8-108">กรอกข้อมูลสำหรับผู้ใช้และตรวจสอบให้แน่ใจว่าภายใต้สิทธิ์การใช้งาน **ผลิตภัณฑ์**สิทธิ์การใช้งานจะถูกกำหนดและ **SharePoint Online** ถูกเลือกไว้</span><span class="sxs-lookup"><span data-stu-id="c36a8-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="c36a8-109">โปรดทราบว่าถ้าคุณอนุญาตให้มีการแชร์ภายนอกในองค์กรของคุณผู้ใช้สามารถแชร์เนื้อหา SharePoint และ OneDrive กับบุคคลภายนอกองค์กรได้</span><span class="sxs-lookup"><span data-stu-id="c36a8-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="c36a8-110">คุณไม่จำเป็นต้องให้สิทธิ์การใช้งานผู้ใช้ภายนอกเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="c36a8-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="c36a8-111">นอกจากนี้คุณยังไม่จำเป็นต้องเพิ่มบัญชีผู้ใช้เหล่านั้นเว้นแต่การแชร์ถูกตั้งค่าเป็น "เฉพาะผู้ใช้ภายนอกที่มีอยู่แล้ว"</span><span class="sxs-lookup"><span data-stu-id="c36a8-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="c36a8-112">ในกรณีนี้ถ้าบุคคลนั้นไม่ได้อยู่ในไดเรกทอรีขององค์กรของคุณคุณจำเป็นต้องเพิ่มบุคคลเหล่านั้นเป็นผู้ใช้ที่เป็นผู้เยี่ยมชมในศูนย์การจัดการ AD Azure</span><span class="sxs-lookup"><span data-stu-id="c36a8-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

