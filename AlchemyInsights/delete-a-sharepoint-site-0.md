---
title: การลบไซต์ SharePoint
ms.author: stevhord
author: bentoncity
manager: scotv
ms.date: 7/30/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4a71f3cd-000a-4a1a-b42a-15b70a8fb6f8
ms.openlocfilehash: 19033fe2f700e940432428e212a5956fcc06b0e6
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36514087"
---
# <a name="delete-sites-that-belong-to-an-office-365-group"></a><span data-ttu-id="ea232-102">ลบไซต์ที่เป็นสมาชิกของกลุ่ม Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="ea232-102">Delete sites that belong to an Office 365 group</span></span>

<span data-ttu-id="ea232-103">เมื่อผู้ใช้สร้างไซต์ทีมใหม่จาก SharePoint Home หรือคุณสร้างไซต์ทีมใหม่จากศูนย์กลางการดูแล SharePoint ใหม่กลุ่ม Office ๓๖๕ที่สอดคล้องกันจะถูกสร้างขึ้นโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="ea232-103">When users create a new team site from SharePoint Home or you create a new team site from the new SharePoint admin center, a corresponding Office 365 group is automatically created.</span></span> <span data-ttu-id="ea232-104">กลุ่ม office ๓๖๕ไซต์ทีมที่เชื่อมต่อจะถูกสร้างขึ้นเมื่อคุณสร้างกลุ่ม Office ๓๖๕หรือทีมงานใน Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ea232-104">Office 365 group-connected team sites are also created when you create an Office 365 group or a team in Microsoft Teams.</span></span> <span data-ttu-id="ea232-105">การลบไซต์ SharePoint ที่เป็นสมาชิกของกลุ่ม Office ๓๖๕คุณจำเป็นต้องลบกลุ่ม Office ๓๖๕ตัวเอง</span><span class="sxs-lookup"><span data-stu-id="ea232-105">To delete a SharePoint site that belongs to an Office 365 group, you need to delete the Office 365 group itself.</span></span> 
  
1. <span data-ttu-id="ea232-106">ไปที่[หน้ากลุ่มของศูนย์ดูแลของ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="ea232-106">Go to the [Groups page of the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/groups).</span></span>
    
2. <span data-ttu-id="ea232-107">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="ea232-107">Select the check box next to the group.</span></span>
    
3. <span data-ttu-id="ea232-108">เลือก**ลบ**</span><span class="sxs-lookup"><span data-stu-id="ea232-108">Select **Delete**.</span></span>
    
<span data-ttu-id="ea232-109">หมายเหตุ: เมื่อคุณลบกลุ่มอาจมีการหน่วงเวลาก่อนที่ไซต์จะถูกเอาออกจาก SharePoint</span><span class="sxs-lookup"><span data-stu-id="ea232-109">NOTE: When you delete a group, there can be a delay before the site is removed from SharePoint.</span></span>
  
<span data-ttu-id="ea232-110">**ลบไซต์การสื่อสารหรือไซต์คลาสสิก:**</span><span class="sxs-lookup"><span data-stu-id="ea232-110">**Delete communication sites or classic sites:**</span></span>

1. <span data-ttu-id="ea232-111">ไปที่เว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="ea232-111">Go to the site.</span></span>
  
2. <span data-ttu-id="ea232-112">คลิกไอคอน**การตั้งค่า**ที่ด้านขวาบน</span><span class="sxs-lookup"><span data-stu-id="ea232-112">Click the **Settings** icon in the upper right.</span></span> 
  
3. <span data-ttu-id="ea232-113">คลิกการ**ตั้งค่าไซต์**</span><span class="sxs-lookup"><span data-stu-id="ea232-113">Click **Site settings**.</span></span> <span data-ttu-id="ea232-114">ภายใต้ข้อ**มูลไซต์**หรือ**การดำเนินการของไซต์**คลิ**กลบไซต์นี้**และจากนั้นคลิ**กลบ**</span><span class="sxs-lookup"><span data-stu-id="ea232-114">Under **Site Information** or **Site Actions**, click **Delete this site**, and then click **Delete**.</span></span>
  
<span data-ttu-id="ea232-115">**ลบไซต์คอลเลกชัน SharePoint:**</span><span class="sxs-lookup"><span data-stu-id="ea232-115">**Delete a SharePoint site collection:**</span></span>

<span data-ttu-id="ea232-116">หากต้องการลบไซต์:</span><span class="sxs-lookup"><span data-stu-id="ea232-116">To delete a site:</span></span>
  
1. <span data-ttu-id="ea232-117">ในศูนย์กลางการดูแล SharePoint ใหม่บนหน้าไซต์ให้คลิ**กกล่องกาเครื่องหมาย**ถัดจากไซต์ที่คุณต้องการลบ</span><span class="sxs-lookup"><span data-stu-id="ea232-117">In the new SharePoint admin center, on the Sites page, click the **check box** next to the site you want to delete.</span></span> 
    
2. <span data-ttu-id="ea232-118">บนแถบเครื่องมือ ribbon คลิ**กลบ**</span><span class="sxs-lookup"><span data-stu-id="ea232-118">On the ribbon toolbar, click **Delete.**</span></span>
    
<span data-ttu-id="ea232-119">**ลบเว็บไซต์โดยบังเอิญ?**</span><span class="sxs-lookup"><span data-stu-id="ea232-119">**Deleted a site by accident?**</span></span>

<span data-ttu-id="ea232-120">โปรดดู[ที่การคืนค่าไซต์คอลเลกชันที่ถูกลบ](https://go.microsoft.com/fwlink/?linkid=867660)</span><span class="sxs-lookup"><span data-stu-id="ea232-120">See [Restore a deleted site collection](https://go.microsoft.com/fwlink/?linkid=867660).</span></span>
  

