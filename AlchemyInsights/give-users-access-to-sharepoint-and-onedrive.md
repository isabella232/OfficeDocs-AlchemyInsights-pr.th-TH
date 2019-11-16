---
title: การให้สิทธิ์การเข้าถึง SharePoint และ OneDrive แก่ผู้ใช้
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
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "36523782"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="b83e4-102">การให้สิทธิ์การเข้าถึง SharePoint และ OneDrive แก่ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="b83e4-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="b83e4-103">ถ้าเว็บไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึงอาจมีปัญหาการบริการแบบถาวร</span><span class="sxs-lookup"><span data-stu-id="b83e4-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="b83e4-104">ตรวจสอบแดชบอร์ดความสมบูรณ์ของบริการ</span><span class="sxs-lookup"><span data-stu-id="b83e4-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="b83e4-105">ถ้าคุณต้องการให้บุคคลในองค์กรของคุณสามารถเข้าสู่ระบบและใช้ SharePoint และ OneDrive คุณจำเป็นต้องเพิ่มบัญชีสำหรับพวกเขาและตรวจสอบให้แน่ใจว่าพวกเขามีสิทธิ์การใช้งานที่ให้พวกเขาเข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="b83e4-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="b83e4-106">วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้อยู่ในศูนย์ดูแลของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="b83e4-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="b83e4-107">ไปที่[เพจที่ผู้ใช้ที่ใช้งานอยู่ในศูนย์ดูแลของ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/users)และจากนั้นคลิ**กเพิ่มผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="b83e4-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="b83e4-108">กรอกข้อมูลสำหรับผู้ใช้และตรวจสอบให้แน่ใจว่าภายใต้**ใบอนุญาตผลิตภัณฑ์**ที่ได้รับการกำหนดสิทธิ์การใช้งานและมีการเลือก**SharePoint แบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="b83e4-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="b83e4-109">โปรดทราบว่าถ้าคุณอนุญาตให้มีการใช้งานร่วมกันภายนอกในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="b83e4-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="b83e4-110">คุณไม่จำเป็นต้องให้ใบอนุญาตผู้ใช้ภายนอกเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="b83e4-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="b83e4-111">นอกจากนี้คุณยังไม่จำเป็นต้องเพิ่มบัญชีสำหรับพวกเขาเว้นแต่จะมีการตั้งค่าการแชร์เป็น "ผู้ใช้ภายนอกที่มีอยู่เท่านั้น"</span><span class="sxs-lookup"><span data-stu-id="b83e4-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="b83e4-112">ในกรณีนี้ถ้าผู้คนไม่ได้อยู่ในไดเรกทอรีขององค์กรคุณจำเป็นต้องเพิ่มเป็นผู้ใช้ที่เป็นแขกในศูนย์ดูแลโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="b83e4-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

