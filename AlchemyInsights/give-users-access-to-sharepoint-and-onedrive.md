---
title: ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 5a1cdeefa4474e8ce0e6a7a37be016cc87b9791d
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498033"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="8d405-102">ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="8d405-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="8d405-p101">ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้ มีการเข้าถึงไซต์ SharePoint หรือการ OneDrive อาจมีปัญหากับบริการชั่วคราว [ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="8d405-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="8d405-p102">ถ้าคุณต้องการให้คนในองค์กรของคุณเพื่อให้สามารถเข้าสู่ระบบ และใช้ SharePoint และ OneDrive คุณจำเป็นต้องเพิ่มบัญชีนั้น และให้แน่ใจว่า พวกเขามีสิทธิ์การใช้งานที่ให้ความเข้ากับ SharePoint และ OneDrive วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้ใน Office 365 admin ศูนย์อยู่</span><span class="sxs-lookup"><span data-stu-id="8d405-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="8d405-107">ไป[หน้าผู้ใช้ที่ใช้งานอยู่ใน Office 365 admin ศูนย์](https://portal.office.com/adminportal/home#/users)และจากนั้น คลิก**เพิ่มผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="8d405-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="8d405-108">กรอกข้อมูลสำหรับผู้ใช้ และให้แน่ ใจว่า ภายใต้**ใบอนุญาตของผลิตภัณฑ์**มีกำหนดสิทธิ์การใช้งาน**แบบออนไลน์ของ SharePoint**ถูกเลือก</span><span class="sxs-lookup"><span data-stu-id="8d405-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="8d405-p103">หมายเหตุว่า ถ้าคุณอนุญาตให้ใช้ร่วมกันในองค์กรภายนอก ผู้ใช้สามารถ SharePoint และ OneDrive ใช้เนื้อหาร่วมกันกับบุคคลภายนอกองค์กร คุณไม่ต้องการให้สิทธิ์การใช้งานของผู้ใช้ภายนอกเหล่านี้ คุณยังไม่จำเป็นต้องเพิ่มบัญชีนั้น ยกเว้นว่ามีการใช้ร่วมกันถูกกำหนดเป็น "เท่านั้นที่มีอยู่แล้วผู้ใช้ภายนอก" ในกรณีดังกล่าว ถ้าบุคคลที่ไม่ได้อยู่ในไดเรกทอรีขององค์กรของคุณ คุณต้องเพิ่มเป็นผู้ใช้แขกในศูนย์ดูแลการโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="8d405-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

