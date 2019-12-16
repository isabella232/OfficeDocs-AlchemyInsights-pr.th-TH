---
title: การแก้ไขปัญหาการเข้าถึงข้อความที่ถูกปฏิเสธไปยัง OneDrive สำหรับไซต์ธุรกิจ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051624"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="19e7f-102">การแก้ไขปัญหาการเข้าถึงข้อความที่ถูกปฏิเสธไปยัง OneDrive สำหรับไซต์ธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="19e7f-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="19e7f-103">ปัญหานี้มักเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="19e7f-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="19e7f-104">บัญชีใหม่จะถูกสร้างขึ้นโดยใช้ค่า PUID (รหัสเฉพาะที่ไม่ซ้ำกัน)</span><span class="sxs-lookup"><span data-stu-id="19e7f-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="19e7f-105">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="19e7f-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="19e7f-106">สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กรไดเรกทอรีที่ใช้งานอยู่ (OU)</span><span class="sxs-lookup"><span data-stu-id="19e7f-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="19e7f-107">ถ้าผู้ใช้มีการลงชื่อเข้าสู่ SharePoint แล้วและถูกย้ายไปยัง OU ที่แตกต่างกันและทำซ้ำกับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="19e7f-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="19e7f-108">เพื่อแก้ไขปัญหานี้คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Office ๓๖๕](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="19e7f-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="19e7f-109">ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมคุณควรเอาผู้ใช้เก่าจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้[เอาผู้ใช้ออกจากรายการข้อมูลผู้ใช้]()</span><span class="sxs-lookup"><span data-stu-id="19e7f-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="19e7f-110">หลังจากนี้เสร็จสิ้นคุณสามารถตรวจสอบผู้ใช้มีสิทธิ์ของผู้ดูแลระบบไปยังไซต์ OneDrive ได้โดยทำตามขั้นตอนเพื่อ[เพิ่มผู้ดูแลสำหรับ OneDrive ของ](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)คุณ</span><span class="sxs-lookup"><span data-stu-id="19e7f-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="19e7f-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ให้ดูบทความให้[เข้าใจระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="19e7f-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
