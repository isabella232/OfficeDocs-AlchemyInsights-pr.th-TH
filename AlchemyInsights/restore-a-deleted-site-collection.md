---
title: คืนค่าไซต์ถูกลบไปแล้ว
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
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369841"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="428d4-102">คืนค่าไซต์ถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="428d4-102">Restore a deleted site</span></span>

<span data-ttu-id="428d4-103">เมื่อผู้ดูแลระบบการลบไซต์ ถูกวางไว้ในไซต์คอลเลกชันถังรีไซเคิล ซึ่งจะถูกเก็บอยู่ 93 วันก่อนที่จะถูกลบออกอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="428d4-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="428d4-104">เมื่อต้องการคืนค่าไซต์:</span><span class="sxs-lookup"><span data-stu-id="428d4-104">To restore the site:</span></span>
  
1. <span data-ttu-id="428d4-105">ในศูนย์การดูแล SharePoint ใหม่คลิก **'ถังรีไซเคิล'** ใน ribbon</span><span class="sxs-lookup"><span data-stu-id="428d4-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="428d4-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="428d4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="428d4-107">คลิก**เรียกคืนรายการที่ถูกลบไปแล้ว**</span><span class="sxs-lookup"><span data-stu-id="428d4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="428d4-108">เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบไปแล้ว คุณสามารถใช้ศูนย์กลางการดูแล SharePoint ใหม่</span><span class="sxs-lookup"><span data-stu-id="428d4-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="428d4-109">มิฉะนั้น คุณจำเป็นต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="428d4-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="428d4-110">เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่มมี Office 365 คุณต้องคืนค่ากลุ่มในศูนย์ดูแลการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="428d4-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="428d4-111">กลุ่มสามารถคืนค่าได้เท่ากับ 30 วันหลังจากที่พวกเขากำลังถูกลบ</span><span class="sxs-lookup"><span data-stu-id="428d4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

