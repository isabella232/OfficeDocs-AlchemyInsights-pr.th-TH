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
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767268"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="360b2-102">แก้ไขปัญหาการแชร์เนื้อหา SharePoint กับผู้ใช้ภายนอก</span><span class="sxs-lookup"><span data-stu-id="360b2-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="360b2-103">ตรวจสอบว่าการใช้ร่วมกันภายนอกเปิดอยู่สําหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="360b2-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="360b2-104">ไปที่หน้า[&amp;บริการเพิ่มเติม ใน ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)และคลิก**ไซต์**หน้า ไซต์ หน้า ไซต์</span><span class="sxs-lookup"><span data-stu-id="360b2-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="360b2-105">ตรวจสอบให้แน่ใจว่าการตั้งค่าถูกเปิดเป็น "เปิด"</span><span class="sxs-lookup"><span data-stu-id="360b2-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="360b2-106">ถ้าเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่"</span><span class="sxs-lookup"><span data-stu-id="360b2-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="360b2-107">ตรวจสอบให้แน่ใจว่าการใช้ร่วมกันภายนอกนั้นเปิดอยู่สําหรับไซต์</span><span class="sxs-lookup"><span data-stu-id="360b2-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="360b2-108">สําหรับไซต์คอลเลกชันแบบคลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="360b2-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="360b2-109">ในศูนย์การจัดการ SharePoint ใหม่ ในบานหน้าต่างด้านซ้าย ให้คลิก**ไซต์**</span><span class="sxs-lookup"><span data-stu-id="360b2-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="360b2-110">เลือกไซต์หรือไซต์ และบน Ribbon ให้คลิก**การใช้ร่วมกัน**</span><span class="sxs-lookup"><span data-stu-id="360b2-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="360b2-111">สําหรับไซต์ทีมที่เป็นสมาชิกของกลุ่ม Office 365 หรือไซต์การติดต่อสื่อสาร ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="360b2-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="360b2-112">ไซต์ประเภทนี้ใหม่มีการตั้งค่าการแชร์แบบเดียวกันเป็นการตั้งค่าทั่วทั้งองค์กรของคุณ ยกเว้นการตั้งค่าทั่วทั้งองค์กรจะอนุญาตให้ใช้แฟ้มร่วมกันโดยใช้ลิงก์ที่ไม่ต้องลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="360b2-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="360b2-113">ในกรณีนี้ ไซต์อนุญาตให้มีการแชร์กับผู้ใช้ภายนอกใหม่และที่มีอยู่ที่ลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="360b2-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="360b2-114">เมื่อต้องการเปลี่ยนการตั้งค่าสําหรับไซต์ที่ระบุ ให้ใช้ศูนย์การจัดการ SharePoint ใหม่หรือ PowerShell</span><span class="sxs-lookup"><span data-stu-id="360b2-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="360b2-115">[เรียนรู้เพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="360b2-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="360b2-116">การตั้งค่าการแชร์ภายนอกสําหรับไซต์ใดๆ อาจจํากัดการตั้งค่าทั่วทั้งองค์กรของคุณได้ มากกว่าการตั้งค่าแบบกว้างขององค์กร แต่จะไม่อนุญาตมากกว่าการตั้งค่าทั่วทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="360b2-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

