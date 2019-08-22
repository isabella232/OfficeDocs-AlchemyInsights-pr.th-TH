---
title: การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503563"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="44512-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์กลางการดูแล Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="44512-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="44512-103">หากคุณได้รับการเข้าถึงถูกปฏิเสธข้อความเมื่อคุณพยายามเรียกดูไปยังศูนย์ดูแล Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณ[มอบหมายสิทธิ์ให้กับผู้ใช้](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="44512-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="44512-104">ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรทำแน่ใจว่า[กำหนดบทบาทเป็นผู้ดูแลระบบ](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ที่สามารถเข้าถึงศูนย์การดูแลด้วย</span><span class="sxs-lookup"><span data-stu-id="44512-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="44512-105">ปัญหานี้สามารถเกิดขึ้นเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN)</span><span class="sxs-lookup"><span data-stu-id="44512-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="44512-106">สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="44512-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="44512-107">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="44512-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="44512-108">สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU)</span><span class="sxs-lookup"><span data-stu-id="44512-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="44512-109">ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="44512-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="44512-110">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ[การคืนค่าผู้ใช้ใน Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="44512-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="44512-111">หมายเหตุ: ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงไว้ก่อนหน้านี้ เป็นศูนย์ OneDrive หรือผู้ดูแลระบบ SharePoint อาจมีปัญหาการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="44512-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="44512-112">[ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="44512-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


