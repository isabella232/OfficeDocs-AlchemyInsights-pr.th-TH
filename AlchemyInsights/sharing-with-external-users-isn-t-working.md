---
title: ใช้ร่วมกันกับผู้ใช้ภายนอกไม่ทำงาน
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900910"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e3c01-102">แก้ไขปัญหาเนื้อหา SharePoint การใช้ร่วมกันกับผู้ใช้ภายนอก</span><span class="sxs-lookup"><span data-stu-id="e3c01-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e3c01-103">ตรวจสอบให้แน่ใจว่า มีการใช้ร่วมกันภายนอกเปิดอยู่สำหรับองค์กรของคุณ:</span><span class="sxs-lookup"><span data-stu-id="e3c01-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e3c01-104">ไป[บริการ&amp;หน้าเพิ่มเติมใน Office 365 admin ศูนย์](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="e3c01-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e3c01-p101">ตรวจสอบว่า มีเปิดการตั้งค่าการ "บน" ถ้ามีเลือก "เท่านั้นที่มีอยู่แล้วผู้ใช้ภายนอก" ต้องแน่ใจว่า ผู้ใช้ภายนอกอยู่ใน Office 365 admin ศูนย์</span><span class="sxs-lookup"><span data-stu-id="e3c01-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="e3c01-p102">ตรวจสอบว่า ภายนอกที่ใช้ร่วมกันจะเปิดใช้งานสำหรับไซต์นี้ สำหรับคลาสสิไซต์คอลเลกชัน:</span><span class="sxs-lookup"><span data-stu-id="e3c01-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="e3c01-109">ในแบบคลาสสิก SharePoint admin ศูนย์ ในบานหน้าต่างด้านซ้าย คลิก**ไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="e3c01-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="e3c01-110">เลือกไซต์หรือไซต์ บน ribbon คลิ ก**ใช้ร่วมกัน**</span><span class="sxs-lookup"><span data-stu-id="e3c01-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e3c01-111">ไซต์สำหรับทีมที่เป็นสมาชิกของกลุ่มมี Office 365 หรือไซต์สื่อสาร:</span><span class="sxs-lookup"><span data-stu-id="e3c01-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e3c01-p103">ชนิดของไซต์เหล่านี้ใหม่ได้แบบเดียวกันร่วมกันการตั้งค่าเป็นการตั้งค่าทั่วทั้งองค์กร ยกเว้นว่ามีการตั้งค่าทั่วทั้งองค์กรอนุญาตให้ใช้ร่วมกันแฟ้มโดยใช้การเชื่อมโยงที่ไม่จำเป็นต้องเข้าสู่ระบบ ในกรณีนี้ ไซต์อนุญาตให้ใช้ร่วมกับที่มีอยู่ และใหม่ภายนอกผู้ใช้ที่เข้าสู่ระบบ เมื่อต้องการเปลี่ยนการตั้งค่าสำหรับไซต์ที่เฉพาะเจาะจง ใช้ศูนย์ดูแล SharePoint ใหม่ (ตัวอย่าง) หรือ PowerShell [ศึกษาเพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="e3c01-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e3c01-116">การตั้งค่าที่ใช้ร่วมกันที่ภายนอกสำหรับไซต์ใด ๆ ก็ได้เข้มงวดมากขึ้นกว่าการตั้งค่าทั่วทั้งองค์กร แต่อ่านไม่มากขึ้นกว่าการตั้งค่าทั่วทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="e3c01-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

