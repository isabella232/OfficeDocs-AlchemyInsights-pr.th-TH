---
title: การแชร์กับผู้ใช้ภายนอกไม่ทํางาน
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582794"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="698ed-102">แก้ไขปัญหาการแชร์เนื้อหา SharePoint กับผู้ใช้ภายนอก</span><span class="sxs-lookup"><span data-stu-id="698ed-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="698ed-103">ตรวจสอบให้แน่ใจว่าเปิดการแชร์ภายนอกสําหรับองค์กรของคุณแล้ว</span><span class="sxs-lookup"><span data-stu-id="698ed-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="698ed-104">ไปที่หน้า[ &amp; Add-in ของบริการในศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)แล้วคลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="698ed-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="698ed-105">ตรวจสอบให้แน่ใจว่าการตั้งค่าถูกเปิดเป็น "เปิด"</span><span class="sxs-lookup"><span data-stu-id="698ed-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="698ed-106">ถ้าเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่" ตรวจสอบให้แน่ใจว่า ผู้ใช้ภายนอกแสดงอยู่ในศูนย์การจัดการ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="698ed-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="698ed-107">ตรวจสอบให้แน่ใจว่าเปิดการแชร์ภายนอกสําหรับไซต์</span><span class="sxs-lookup"><span data-stu-id="698ed-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="698ed-108">สําหรับไซต์คอลเลกชันแบบคลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="698ed-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="698ed-109">ในศูนย์การจัดการ SharePoint ใหม่ ในบานหน้าต่างด้านซ้าย ให้คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="698ed-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="698ed-110">เลือกไซต์หรือไซต์ และบน Ribbon ให้คลิก**การใช้ร่วมกัน**</span><span class="sxs-lookup"><span data-stu-id="698ed-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="698ed-111">สําหรับไซต์ทีมที่เป็นสมาชิกของกลุ่ม Microsoft 365 หรือไซต์การติดต่อสื่อสาร:</span><span class="sxs-lookup"><span data-stu-id="698ed-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="698ed-112">ไซต์ชนิดใหม่เหล่านี้มีการตั้งค่าการแชร์แบบเดียวกับการตั้งค่าทั่วทั้งองค์กรของคุณ เว้นแต่การตั้งค่าทั้งองค์กรจะอนุญาตให้แชร์ไฟล์โดยใช้ลิงก์ที่ไม่จําเป็นต้องลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="698ed-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="698ed-113">ในกรณีนี้ ไซต์อนุญาตให้แชร์กับผู้ใช้ภายนอกใหม่และที่มีอยู่ซึ่งลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="698ed-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="698ed-114">เมื่อต้องการเปลี่ยนการตั้งค่าสําหรับไซต์เฉพาะ ให้ใช้ศูนย์การจัดการ SharePoint ใหม่หรือ PowerShell</span><span class="sxs-lookup"><span data-stu-id="698ed-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="698ed-115">[ดูเพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="698ed-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="698ed-116">การตั้งค่าการแชร์ภายนอกสําหรับไซต์ใดๆ อาจจํากัดมากกว่าการตั้งค่าทั่วทั้งองค์กรของคุณ แต่ไม่อนุญาตมากกว่าการตั้งค่าทั่วทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="698ed-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

