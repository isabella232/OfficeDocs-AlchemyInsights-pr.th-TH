---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยังไซต์ OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670635"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="64fb6-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยังไซต์ OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="64fb6-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="64fb6-103">ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="64fb6-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="64fb6-104">บัญชีผู้ใช้ใหม่ถูกสร้างโดยใช้ค่า PUID (ID ที่ไม่ซ้ำกันของ Passport) ที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="64fb6-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="64fb6-105">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="64fb6-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="64fb6-106">สถานการณ์สมมติที่สองจะเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีกับหน่วยองค์กร Active Directory (OU)</span><span class="sxs-lookup"><span data-stu-id="64fb6-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="64fb6-107">ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint เรียบร้อยแล้วและจะถูกย้ายไปยัง OU และ resynced ที่แตกต่างกันกับ SharePoint พวกเขาอาจประสบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="64fb6-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="64fb6-108">เมื่อต้องการแก้ไขปัญหานี้คุณควรคืนค่า UPN ต้นฉบับที่มีขั้นตอนในบทความให้[คืนค่าผู้ใช้ใน Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="64fb6-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="64fb6-109">ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิมที่คุณควรเอาผู้ใช้เก่าออกจากไซต์ OneDrive โดยใช้ขั้นตอนเหล่านี้ให้[เอาผู้ใช้ออกจากรายการข้อมูลผู้ใช้]()</span><span class="sxs-lookup"><span data-stu-id="64fb6-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="64fb6-110">หลังจากเสร็จเรียบร้อยแล้วคุณสามารถตรวจสอบว่าผู้ใช้มีสิทธิ์ผู้ดูแลระบบไปยังไซต์ OneDrive โดยทำตามขั้นตอนในการ [เพิ่มผู้ดูแลระบบสำหรับ onedrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="64fb6-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="64fb6-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ให้ดูบทความการ[ทำความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="64fb6-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
