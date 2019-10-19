---
title: กู้คืนไซต์ที่ถูกลบ
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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36552500"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="c7382-102">กู้คืนไซต์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="c7382-102">Restore a deleted site</span></span>

<span data-ttu-id="c7382-103">เมื่อผู้ดูแลลบไซต์จะถูกวางไว้ในไซต์คอลเลกชันถังรีไซเคิลซึ่งจะถูกเก็บไว้เป็นเวลา๙๓วันก่อนที่จะถูกลบอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="c7382-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="c7382-104">หากต้องการคืนค่าไซต์ให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="c7382-104">To restore the site:</span></span>
  
1. <span data-ttu-id="c7382-105">ในศูนย์กลางการดูแล SharePoint ใหม่คลิก**ถังรีไซเคิล**บน ribbon</span><span class="sxs-lookup"><span data-stu-id="c7382-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="c7382-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากชุดเก็บรวบรวมไซต์ที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="c7382-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="c7382-107">คลิ**กกู้คืนรายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="c7382-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="c7382-108">ในการคืนค่าไซต์การสื่อสารที่ถูกลบคุณสามารถใช้ศูนย์กลางการดูแล SharePoint ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="c7382-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="c7382-109">มิฉะนั้นคุณต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="c7382-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="c7382-110">ในการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Office ๓๖๕คุณจำเป็นต้องคืนค่ากลุ่มในศูนย์ดูแล Exchange</span><span class="sxs-lookup"><span data-stu-id="c7382-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="c7382-111">คุณสามารถกู้คืนกลุ่มได้เป็นเวลา30วันหลังจากที่ลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="c7382-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

