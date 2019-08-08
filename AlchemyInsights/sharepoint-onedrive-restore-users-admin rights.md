---
title: การแก้ไขปัญหาการเข้าถึงปฏิเสธข้อความ OneDrive สำหรับไซต์ทางธุรกิจ
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232563"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="07e98-102">การแก้ไขปัญหาการเข้าถึงปฏิเสธข้อความ OneDrive สำหรับไซต์ทางธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="07e98-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="07e98-103">ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN)</span><span class="sxs-lookup"><span data-stu-id="07e98-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="07e98-104">สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="07e98-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="07e98-105">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="07e98-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="07e98-106">สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU)</span><span class="sxs-lookup"><span data-stu-id="07e98-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="07e98-107">ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="07e98-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="07e98-108">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ[การคืนค่าผู้ใช้ใน Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="07e98-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="07e98-109">ถ้าคุณไม่สามารถคืนค่าที่ผู้ใช้เดิม คุณควรเก่าเอาผู้ใช้ออกจากไซต์ OneDrive โดยใช้ขั้นตอนต่อไป[เอาผู้ใช้จากรายการข้อมูลผู้ใช้]()</span><span class="sxs-lookup"><span data-stu-id="07e98-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="07e98-110">หลังจากทำเช่นนี้ คุณสามารถตรวจสอบว่า ผู้ใช้มีสิทธิ์การดูแลไปยังไซต์ OneDrive โดยทำตามขั้นตอนเพื่อ[เพิ่ม admin ของสำหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="07e98-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="07e98-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ดูบทความ[การทำความเข้าใจระดับของสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="07e98-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
