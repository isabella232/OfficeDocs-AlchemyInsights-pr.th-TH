---
title: การแชร์กับผู้ใช้ภายนอกไม่ทำงาน
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502250"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="a4e60-102">แก้ไขปัญหาในการใช้เนื้อหา SharePoint ร่วมกับบุคคลภายนอก</span><span class="sxs-lookup"><span data-stu-id="a4e60-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="a4e60-103">ตรวจสอบให้แน่ใจว่าการแชร์ภายนอกเปิดอยู่สำหรับองค์กรของคุณ:</span><span class="sxs-lookup"><span data-stu-id="a4e60-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="a4e60-104">ไปที่[หน้าเพิ่ม&amp;เติมของบริการในศูนย์ดูแลของ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)และคลิ**กไซต์**</span><span class="sxs-lookup"><span data-stu-id="a4e60-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="a4e60-105">ตรวจสอบให้แน่ใจว่าการตั้งค่าถูกเปิด "เปิด"</span><span class="sxs-lookup"><span data-stu-id="a4e60-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="a4e60-106">ถ้าเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่" เท่านั้นให้ตรวจสอบให้แน่ใจว่าผู้ใช้ภายนอกจะแสดงอยู่ในศูนย์ดูแลของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="a4e60-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="a4e60-107">ตรวจสอบให้แน่ใจว่าการใช้งานร่วมกันภายนอกเปิดอยู่สำหรับไซต์</span><span class="sxs-lookup"><span data-stu-id="a4e60-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="a4e60-108">สำหรับไซต์คอลเลกชันคลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="a4e60-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="a4e60-109">ในศูนย์กลางการดูแล SharePoint ใหม่ในบานหน้าต่างด้านซ้ายให้คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="a4e60-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="a4e60-110">เลือกไซต์หรือไซต์และบน ribbon คลิกการใช้**ร่วมกัน**</span><span class="sxs-lookup"><span data-stu-id="a4e60-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="a4e60-111">สำหรับไซต์ทีมที่เป็นสมาชิกของกลุ่ม Office ๓๖๕หรือไซต์การสื่อสาร:</span><span class="sxs-lookup"><span data-stu-id="a4e60-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="a4e60-112">ชนิดของไซต์ใหม่เหล่านี้มีการตั้งค่าการใช้ร่วมกันแบบเดียวกับการตั้งค่าทั่วทั้งองค์กรของคุณเว้นแต่การตั้งค่าทั่วทั้งองค์กรอนุญาตให้ใช้แฟ้มร่วมกันด้วยการเชื่อมโยงที่ไม่จำเป็นต้องเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="a4e60-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="a4e60-113">ในกรณีนี้เว็บไซต์อนุญาตให้แชร์กับผู้ใช้ภายนอกที่มีอยู่และใหม่ที่ลงชื่อเข้าใช้ได้</span><span class="sxs-lookup"><span data-stu-id="a4e60-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="a4e60-114">หากต้องการเปลี่ยนแปลงการตั้งค่าสำหรับไซต์ที่ระบุให้ใช้ศูนย์กลางการดูแล SharePoint หรือ PowerShell ใหม่</span><span class="sxs-lookup"><span data-stu-id="a4e60-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="a4e60-115">[เรียนรู้เพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="a4e60-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="a4e60-116">การตั้งค่าการใช้ร่วมกันภายนอกสำหรับไซต์ใดๆสามารถมีความเข้มงวดมากกว่าการตั้งค่าทั่วทั้งองค์กรของคุณแต่ไม่ได้มากกว่าการตั้งค่าทั่วทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="a4e60-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

