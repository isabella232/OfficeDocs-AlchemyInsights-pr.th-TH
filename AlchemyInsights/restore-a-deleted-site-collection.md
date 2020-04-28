---
title: คืนค่าไซต์ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912694"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="3bd43-102">คืนค่าไซต์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="3bd43-102">Restore a deleted site</span></span>

<span data-ttu-id="3bd43-103">เมื่อผู้ดูแลระบบลบไซต์ SharePoint ไซต์นั้นจะถูกวางไว้ในถังรีไซเคิลของไซต์คอลเลกชัน ซึ่งถูกเก็บไว้เป็นเวลา 93 วันก่อนที่จะถูกลบอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="3bd43-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="3bd43-104">เมื่อต้องการคืนค่าไซต์:</span><span class="sxs-lookup"><span data-stu-id="3bd43-104">To restore the site:</span></span>
  
1. <span data-ttu-id="3bd43-105">ในศูนย์การจัดการ SharePoint ใหม่ ให้คลิก**ถังรีไซเคิล**บน Ribbon</span><span class="sxs-lookup"><span data-stu-id="3bd43-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="3bd43-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="3bd43-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="3bd43-107">คลิก**คืนค่ารายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="3bd43-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="3bd43-108">เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="3bd43-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="3bd43-109">มิฉะนั้น คุณจําเป็นต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="3bd43-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="3bd43-110">เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Microsoft 365 คุณต้องคืนค่ากลุ่มในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="3bd43-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="3bd43-111">กลุ่มสามารถเรียกคืนได้เป็นเวลา 30 วันหลังจากที่ลบ</span><span class="sxs-lookup"><span data-stu-id="3bd43-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

