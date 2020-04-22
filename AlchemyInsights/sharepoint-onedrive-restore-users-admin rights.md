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
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692820"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="9944f-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="9944f-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="9944f-103">ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบ และสร้างใหม่ ด้วยชื่อหลัก (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="9944f-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="9944f-104">บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะของ Passport) ที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="9944f-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="9944f-105">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของตนเอง</span><span class="sxs-lookup"><span data-stu-id="9944f-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="9944f-106">สถานการณ์สมมติที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับ Active Directory องค์กรหน่วย (OU)</span><span class="sxs-lookup"><span data-stu-id="9944f-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="9944f-107">ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="9944f-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="9944f-108">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่างๆ ในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="9944f-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="9944f-109">ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมที่คุณควรเอาผู้ใช้เก่าจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้[Remove a user from the user info list]()</span><span class="sxs-lookup"><span data-stu-id="9944f-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="9944f-110">หลังจากเสร็จสิ้นคุณสามารถตรวจสอบว่า ผู้ใช้มีสิทธิ์ของผู้ดูแลระบบไปยังไซต์ OneDrive โดยทําตามขั้นตอนใน[การเพิ่มผู้ดูแลระบบสําหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="9944f-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="9944f-111">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ให้ดูที่บทความ การ[ทําความเข้าใจระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="9944f-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
