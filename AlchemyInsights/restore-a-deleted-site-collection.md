---
title: การคืนค่าไซต์ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692062"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="43d56-102">การคืนค่าไซต์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="43d56-102">Restore a deleted site</span></span>

<span data-ttu-id="43d56-103">เมื่อผู้ดูแลระบบลบไซต์ SharePoint แล้วไฟล์นั้นจะถูกวางไว้ในถังรีไซเคิลของไซต์คอลเลกชันซึ่งจะถูกเก็บไว้สำหรับ๙๓วันก่อนที่จะถูกลบออกอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="43d56-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="43d56-104">เมื่อต้องการคืนค่าไซต์:</span><span class="sxs-lookup"><span data-stu-id="43d56-104">To restore the site:</span></span>
  
1. <span data-ttu-id="43d56-105">ในศูนย์การจัดการ SharePoint ใหม่ให้คลิกถัง **รีไซเคิล** บน ribbon</span><span class="sxs-lookup"><span data-stu-id="43d56-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="43d56-106">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า</span><span class="sxs-lookup"><span data-stu-id="43d56-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="43d56-107">คลิก**คืนค่ารายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="43d56-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="43d56-108">เมื่อต้องการคืนค่าไซต์การติดต่อสื่อสารที่ถูกลบคุณสามารถใช้ศูนย์การจัดการ SharePoint ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="43d56-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="43d56-109">มิฉะนั้นคุณจำเป็นต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="43d56-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="43d56-110">เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Microsoft ๓๖๕คุณจำเป็นต้องคืนค่ากลุ่มในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="43d56-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="43d56-111">กลุ่มสามารถคืนค่าเป็นเวลา30วันหลังจากที่ถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="43d56-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

