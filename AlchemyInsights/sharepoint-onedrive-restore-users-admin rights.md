---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511203"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="9e7a8-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="9e7a8-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="9e7a8-103">ปัญหานี้ส่วนใหญ่มักเกิดขึ้นเมื่อผู้ใช้จะถูกลบ และสร้างใหม่ ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="9e7a8-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="9e7a8-104">บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะหนังสือเดินทาง) ที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="9e7a8-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="9e7a8-105">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ผู้ใช้มี PUID ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="9e7a8-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="9e7a8-106">สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กร Active Directory (OU)</span><span class="sxs-lookup"><span data-stu-id="9e7a8-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="9e7a8-107">ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="9e7a8-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="9e7a8-108">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="9e7a8-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="9e7a8-109">ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิม[Remove a user from the user info list]()</span><span class="sxs-lookup"><span data-stu-id="9e7a8-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="9e7a8-110">หลังจากเสร็จสิ้นแล้ว คุณสามารถตรวจสอบผู้ใช้มีสิทธิ์ผู้ดูแลระบบในไซต์ OneDrive โดยทําตามขั้นตอนการเพิ่ม[ผู้ดูแลระบบสําหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="9e7a8-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="9e7a8-111">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ให้ดูบทความ[การทําความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="9e7a8-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
