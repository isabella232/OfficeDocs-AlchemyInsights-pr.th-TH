---
title: ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ebb9037362d261b81b9b1dcafcbe461aac7f4963
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759637"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="25bb3-102">ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="25bb3-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="25bb3-103">ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้ มีการเข้าถึงไซต์ SharePoint หรือการ OneDrive อาจมีปัญหากับบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="25bb3-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="25bb3-104">ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ</span><span class="sxs-lookup"><span data-stu-id="25bb3-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="25bb3-105">ถ้าคุณต้องการให้คนในองค์กรของคุณเพื่อให้สามารถเข้าสู่ระบบ และใช้ SharePoint และ OneDrive คุณจำเป็นต้องเพิ่มบัญชีนั้น และให้แน่ใจว่า พวกเขามีสิทธิ์การใช้งานที่ให้ความเข้ากับ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="25bb3-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="25bb3-106">วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้ใน Microsoft 365 admin ศูนย์อยู่</span><span class="sxs-lookup"><span data-stu-id="25bb3-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="25bb3-107">ไป[หน้าผู้ใช้ที่ใช้งานอยู่ใน Microsoft 365 admin ศูนย์](https://portal.office.com/adminportal/home#/users)และจากนั้น คลิก**เพิ่มผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="25bb3-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="25bb3-108">กรอกข้อมูลสำหรับผู้ใช้ และให้แน่ ใจว่า ภายใต้**ใบอนุญาตของผลิตภัณฑ์**มีกำหนดสิทธิ์การใช้งาน**แบบออนไลน์ของ SharePoint**ถูกเลือก</span><span class="sxs-lookup"><span data-stu-id="25bb3-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="25bb3-109">หมายเหตุว่า ถ้าคุณอนุญาตให้ใช้ร่วมกันในองค์กรภายนอก ผู้ใช้สามารถ SharePoint และ OneDrive ใช้เนื้อหาร่วมกันกับบุคคลภายนอกองค์กร</span><span class="sxs-lookup"><span data-stu-id="25bb3-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="25bb3-110">คุณไม่ต้องการให้สิทธิ์การใช้งานของผู้ใช้ภายนอกเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="25bb3-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="25bb3-111">คุณยังไม่จำเป็นต้องเพิ่มบัญชีนั้น ยกเว้นว่ามีการใช้ร่วมกันถูกกำหนดเป็น "เท่านั้นที่มีอยู่แล้วผู้ใช้ภายนอก"</span><span class="sxs-lookup"><span data-stu-id="25bb3-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="25bb3-112">ในกรณีดังกล่าว ถ้าบุคคลที่ไม่ได้อยู่ในไดเรกทอรีขององค์กรของคุณ คุณต้องเพิ่มเป็นผู้ใช้แขกในศูนย์ดูแลการโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="25bb3-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

