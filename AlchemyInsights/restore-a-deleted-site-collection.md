---
title: คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753805"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="5b40f-102">คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="5b40f-102">Restore a deleted site collection</span></span>

<span data-ttu-id="5b40f-103">เมื่อ admin การลบคอลเลกชันไซต์คลาสสิค ถูกวางไว้ในไซต์คอลเลกชันถังรีไซเคิล ซึ่งจะถูกเก็บอยู่ 93 วันก่อนที่จะถูกลบออกอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="5b40f-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="5b40f-104">เมื่อต้องการคืนค่าไซต์คอลเลกชัน:</span><span class="sxs-lookup"><span data-stu-id="5b40f-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="5b40f-105">ในศูนย์ดูแลแบบคลาสสิกของ SharePoint คลิก **'ถังรีไซเคิล'** ใน ribbon</span><span class="sxs-lookup"><span data-stu-id="5b40f-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="5b40f-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="5b40f-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="5b40f-107">คลิก**เรียกคืนรายการที่ถูกลบไปแล้ว**</span><span class="sxs-lookup"><span data-stu-id="5b40f-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="5b40f-108">เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบไปแล้ว คุณสามารถใช้ตัวอย่างศูนย์ดูแล SharePoint ใหม่</span><span class="sxs-lookup"><span data-stu-id="5b40f-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="5b40f-109">มิฉะนั้น คุณจำเป็นต้องใช้ PowerShell</span><span class="sxs-lookup"><span data-stu-id="5b40f-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="5b40f-110">เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่มมี Office 365 คุณต้องคืนค่ากลุ่มในศูนย์ดูแลการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="5b40f-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="5b40f-111">กลุ่มสามารถคืนค่าได้เท่ากับ 30 วันหลังจากที่พวกเขากำลังถูกลบ</span><span class="sxs-lookup"><span data-stu-id="5b40f-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

