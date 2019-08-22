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
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502250"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="85dfb-102">แก้ไขปัญหาเนื้อหา SharePoint การใช้ร่วมกันกับผู้ใช้ภายนอก</span><span class="sxs-lookup"><span data-stu-id="85dfb-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="85dfb-103">ตรวจสอบให้แน่ใจว่า มีการใช้ร่วมกันภายนอกเปิดอยู่สำหรับองค์กรของคุณ:</span><span class="sxs-lookup"><span data-stu-id="85dfb-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="85dfb-104">ไป[บริการ&amp;หน้าเพิ่มเติมใน Microsoft 365 admin ศูนย์](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="85dfb-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="85dfb-105">ตรวจสอบว่า มีเปิดการตั้งค่าการ "บน"</span><span class="sxs-lookup"><span data-stu-id="85dfb-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="85dfb-106">ถ้ามีเลือก "เท่านั้นที่มีอยู่แล้วผู้ใช้ภายนอก" ต้องแน่ใจว่า ผู้ใช้ภายนอกจะอยู่ในศูนย์กลาง Microsoft 365 admin</span><span class="sxs-lookup"><span data-stu-id="85dfb-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="85dfb-107">ตรวจสอบว่า ภายนอกที่ใช้ร่วมกันจะเปิดใช้งานสำหรับไซต์นี้</span><span class="sxs-lookup"><span data-stu-id="85dfb-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="85dfb-108">สำหรับคลาสสิไซต์คอลเลกชัน:</span><span class="sxs-lookup"><span data-stu-id="85dfb-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="85dfb-109">ในใหม่ SharePoint admin ศูนย์ ในบานหน้าต่างด้านซ้าย คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="85dfb-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="85dfb-110">เลือกไซต์หรือไซต์ บน ribbon คลิ ก**ใช้ร่วมกัน**</span><span class="sxs-lookup"><span data-stu-id="85dfb-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="85dfb-111">ไซต์สำหรับทีมที่เป็นสมาชิกของกลุ่มมี Office 365 หรือไซต์สื่อสาร:</span><span class="sxs-lookup"><span data-stu-id="85dfb-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="85dfb-112">ชนิดของไซต์เหล่านี้ใหม่ได้แบบเดียวกันร่วมกันการตั้งค่าเป็นการตั้งค่าทั่วทั้งองค์กร ยกเว้นว่ามีการตั้งค่าทั่วทั้งองค์กรอนุญาตให้ใช้ร่วมกันแฟ้มโดยใช้การเชื่อมโยงที่ไม่จำเป็นต้องเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="85dfb-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="85dfb-113">ในกรณีนี้ ไซต์อนุญาตให้ใช้ร่วมกับที่มีอยู่ และใหม่ภายนอกผู้ใช้ที่เข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="85dfb-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="85dfb-114">เมื่อต้องการเปลี่ยนการตั้งค่าสำหรับไซต์ที่เฉพาะเจาะจง ใช้ศูนย์กลางการดูแล SharePoint ใหม่หรือ PowerShell</span><span class="sxs-lookup"><span data-stu-id="85dfb-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="85dfb-115">[ศึกษาเพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="85dfb-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="85dfb-116">การตั้งค่าที่ใช้ร่วมกันที่ภายนอกสำหรับไซต์ใด ๆ ก็ได้เข้มงวดมากขึ้นกว่าการตั้งค่าทั่วทั้งองค์กร แต่อ่านไม่มากขึ้นกว่าการตั้งค่าทั่วทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="85dfb-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

