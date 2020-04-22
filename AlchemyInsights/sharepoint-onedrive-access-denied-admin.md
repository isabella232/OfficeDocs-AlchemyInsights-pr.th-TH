---
title: การแก้ไขปัญหาข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758539"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="4cd0a-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์การจัดการ Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="4cd0a-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="4cd0a-103">ถ้าคุณได้รับการเข้าถึงถูกปฏิเสธข้อความเมื่อพยายามที่จะเรียกดูไปยังศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่า คุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="4cd0a-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="4cd0a-104">ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[มอบหมายบทบาทผู้ดูแลระบบ](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ที่สามารถเข้าถึงศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="4cd0a-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="4cd0a-105">ปัญหานี้อาจเกิดขึ้นได้เมื่อผู้ใช้ถูกลบ และสร้างใหม่ ด้วยชื่อหลัก (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="4cd0a-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4cd0a-106">บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะของ Passport) ที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="4cd0a-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4cd0a-107">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของตนเอง</span><span class="sxs-lookup"><span data-stu-id="4cd0a-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4cd0a-108">สถานการณ์สมมติที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับ Active Directory องค์กรหน่วย (OU)</span><span class="sxs-lookup"><span data-stu-id="4cd0a-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4cd0a-109">ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="4cd0a-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4cd0a-110">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่างๆ ในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="4cd0a-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="4cd0a-111">หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่เคยมีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="4cd0a-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="4cd0a-112">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="4cd0a-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


