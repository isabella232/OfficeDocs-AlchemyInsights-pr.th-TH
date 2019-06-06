---
title: ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736666"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="7c341-102">ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="7c341-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="7c341-103">ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN)</span><span class="sxs-lookup"><span data-stu-id="7c341-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="7c341-104">สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="7c341-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="7c341-105">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="7c341-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="7c341-106">สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU)</span><span class="sxs-lookup"><span data-stu-id="7c341-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="7c341-107">ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="7c341-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="7c341-108">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ[การคืนค่าผู้ใช้ใน Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7c341-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="7c341-109">หลังจากทำเช่นนี้ คุณสามารถตรวจสอบว่า ผู้ใช้มีสิทธิ์การดูแลไปยังไซต์ OneDrive โดยทำตามขั้นตอนเพื่อ[เพิ่ม admin ของสำหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="7c341-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="7c341-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ดูบทความ[การทำความเข้าใจระดับของสิทธิ์ใน SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="7c341-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
