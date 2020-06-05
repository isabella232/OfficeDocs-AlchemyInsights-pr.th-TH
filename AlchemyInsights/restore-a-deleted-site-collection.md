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
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582254"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="ce5f5-102">คืนค่าไซต์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="ce5f5-102">Restore a deleted site</span></span>

<span data-ttu-id="ce5f5-103">เมื่อผู้ดูแลลบไซต์ SharePoint ไซต์จะถูกวางไว้ในถังรีไซเคิลของไซต์คอลเลกชัน ซึ่งจะถูกเก็บไว้เป็นเวลา 93 วันก่อนที่ไซต์จะถูกลบอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="ce5f5-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="ce5f5-104">เมื่อต้องการคืนค่าไซต์:</span><span class="sxs-lookup"><span data-stu-id="ce5f5-104">To restore the site:</span></span>
  
1. <span data-ttu-id="ce5f5-105">ในศูนย์การจัดการ SharePoint ใหม่ ให้คลิก**ถังรีไซเคิล**บน Ribbon</span><span class="sxs-lookup"><span data-stu-id="ce5f5-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="ce5f5-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="ce5f5-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="ce5f5-107">คลิก**คืนค่ารายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="ce5f5-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="ce5f5-108">เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="ce5f5-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="ce5f5-109">มิฉะนั้น คุณต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="ce5f5-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="ce5f5-110">เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Microsoft 365 คุณจําเป็นต้องคืนค่ากลุ่มในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5f5-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="ce5f5-111">กลุ่มสามารถเรียกคืนได้เป็นเวลา 30 วันหลังจากที่ลบกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="ce5f5-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

