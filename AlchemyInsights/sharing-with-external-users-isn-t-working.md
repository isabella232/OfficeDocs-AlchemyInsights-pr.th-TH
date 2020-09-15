---
title: การแชร์กับผู้ใช้ภายนอกไม่ทำงาน
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691594"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="88479-102">แก้ไขปัญหาการแชร์เนื้อหา SharePoint กับผู้ใช้ภายนอก</span><span class="sxs-lookup"><span data-stu-id="88479-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="88479-103">ตรวจสอบให้แน่ใจว่ามีการเปิดใช้งานการแชร์ภายนอกสำหรับองค์กรของคุณ:</span><span class="sxs-lookup"><span data-stu-id="88479-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="88479-104">ไปที่[ &amp; หน้า Add-in ของบริการในศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)แล้วคลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="88479-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="88479-105">ตรวจสอบให้แน่ใจว่าการตั้งค่าถูกเปิดใช้งาน "เปิด"</span><span class="sxs-lookup"><span data-stu-id="88479-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="88479-106">ถ้ามีการเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่แล้ว" ให้ตรวจสอบให้แน่ใจว่าผู้ใช้ภายนอกแสดงอยู่ในศูนย์การจัดการ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="88479-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="88479-107">ตรวจสอบให้แน่ใจว่าการแชร์ภายนอกเปิดใช้งานสำหรับไซต์แล้ว</span><span class="sxs-lookup"><span data-stu-id="88479-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="88479-108">สำหรับไซต์คอลเลกชันแบบคลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="88479-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="88479-109">ในศูนย์การจัดการ SharePoint ใหม่ในบานหน้าต่างด้านซ้ายให้คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="88479-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="88479-110">เลือกไซต์หรือไซต์และบน ribbon ให้คลิกการ**แชร์**</span><span class="sxs-lookup"><span data-stu-id="88479-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="88479-111">สำหรับไซต์ทีมที่เป็นสมาชิกของกลุ่ม Microsoft ๓๖๕หรือไซต์การติดต่อสื่อสาร:</span><span class="sxs-lookup"><span data-stu-id="88479-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="88479-112">ชนิดไซต์ใหม่เหล่านี้จะมีการตั้งค่าการแชร์เดียวกันกับการตั้งค่าทั้งองค์กรของคุณเว้นแต่การตั้งค่าทั้งองค์กรช่วยให้การใช้ไฟล์ร่วมกันโดยใช้ลิงก์ที่ไม่จำเป็นต้องลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="88479-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="88479-113">ในกรณีนี้ไซต์จะอนุญาตให้มีการแชร์กับผู้ใช้ภายนอกใหม่และผู้ใช้ภายนอกที่มีอยู่แล้วในการลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="88479-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="88479-114">เมื่อต้องการเปลี่ยนการตั้งค่าสำหรับไซต์ที่เฉพาะเจาะจงให้ใช้ศูนย์การจัดการ SharePoint ใหม่หรือ PowerShell</span><span class="sxs-lookup"><span data-stu-id="88479-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="88479-115">[เรียนรู้เพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="88479-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="88479-116">การตั้งค่าการแชร์ภายนอกสำหรับไซต์ใดก็ได้จะเข้มงวดกว่าการตั้งค่าทั้งองค์กรของคุณแต่จะไม่ permissive มากกว่าการตั้งค่าทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="88479-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

