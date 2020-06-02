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
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505398"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="11331-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์การจัดการของ Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="11331-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="11331-103">ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไปยังศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณ[ได้มอบหมายสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="11331-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="11331-104">ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[มอบหมายบทบาทผู้ดูแลระบบ](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles)ที่สามารถเข้าถึงศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="11331-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="11331-105">ปัญหานี้อาจเกิดขึ้นเมื่อผู้ใช้จะถูกลบ และสร้างใหม่ ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="11331-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="11331-106">บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะหนังสือเดินทาง) ที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="11331-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="11331-107">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ผู้ใช้มี PUID ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="11331-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="11331-108">สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กร Active Directory (OU)</span><span class="sxs-lookup"><span data-stu-id="11331-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="11331-109">ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="11331-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="11331-110">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="11331-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="11331-111">หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่เคยเข้าถึงก่อนหน้านี้</span><span class="sxs-lookup"><span data-stu-id="11331-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="11331-112">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="11331-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


