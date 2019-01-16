---
title: คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316511"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="d82d7-102">คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="d82d7-102">Restore a deleted site collection</span></span>

<span data-ttu-id="d82d7-p101">เมื่อ admin การลบคอลเลกชันไซต์คลาสสิค ถูกวางไว้ในไซต์คอลเลกชันถังรีไซเคิล ซึ่งจะถูกเก็บอยู่ 93 วันก่อนที่จะถูกลบออกอย่างถาวร เมื่อต้องการคืนค่าไซต์คอลเลกชัน:</span><span class="sxs-lookup"><span data-stu-id="d82d7-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="d82d7-105">ในศูนย์ดูแลแบบคลาสสิกของ SharePoint คลิก **'ถังรีไซเคิล'** ใน ribbon</span><span class="sxs-lookup"><span data-stu-id="d82d7-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d82d7-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="d82d7-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d82d7-107">คลิก**เรียกคืนรายการที่ถูกลบไปแล้ว**</span><span class="sxs-lookup"><span data-stu-id="d82d7-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d82d7-p102">เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบไปแล้ว คุณสามารถใช้ตัวอย่างศูนย์ดูแล SharePoint ใหม่ มิฉะนั้น คุณจำเป็นต้องใช้ PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่มมี Office 365 คุณต้องคืนค่ากลุ่มในศูนย์ดูแลการแลกเปลี่ยน กลุ่มสามารถคืนค่าได้เท่ากับ 30 วันหลังจากที่พวกเขากำลังถูกลบ</span><span class="sxs-lookup"><span data-stu-id="d82d7-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

